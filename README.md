# Galicia: law history in git

The law of the autonomous community of Galicia (Comunidad Autónoma de Galicia, Spain) as a git history: one file per article, one commit per norm that changed it, dated the day the change took effect, with the amending norm as the commit's author. `git blame` names the norm behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `es-ga/`. Spain's national law is in [lexifina/spain-law](https://github.com/lexifina/spain-law).

The text is in Spanish, exactly as the BOE's consolidated text prints it. Texts in co-official languages are not included.

Basado en datos de la Agencia Estatal Boletín Oficial del Estado (<https://www.boe.es>). Every text here is a consolidated text for information only (texto consolidado de carácter meramente informativo), not an official publication.

## What this repository holds

217 norms with 1020 versions so far: the Estatuto de Autonomía first, then the laws, decree-laws and legislative decrees in force that the BOE consolidates, oldest first, added in parts of about 50. 25 of them are repealed norms the BOE consolidates: their whole history is kept, and their last commit removes the text on the day the repeal took effect, credited to the repealing norm. Regulations are not included (the BOE consolidates no autonomic decrees or orders).

| Folder | Norm | Versions | History | BOE last updated |
| --- | --- | ---: | --- | --- |
| `estatuto-de-autonomia/` | Ley Orgánica 1/1981, de 6 de abril, de Estatuto de Autonomía para Galicia. | 6 | as first published, then each change: 18 May 1981 to 29 December 2022 | 2026-07-31 |
| `ley-1982-001/` | Ley 1/1982, de 24 de junio, por la que se fija la sede de las Instituciones autonómicas de Galicia. | 1 | as first published: 12 August 1982 | 2025-12-16 |
| `ley-1983-001/` | Ley 1/1983, de 22 de febrero, reguladora de la Junta y su Presidente. | 8 | as first published, then each change: 21 March 1983 to 5 September 2015 | 2026-06-26 |
| `ley-1983-003/` | Ley 3/1983, de 15 de junio, de normalización lingüística. | 2 | as first published, then each change: 15 July 1983 to 4 July 1986 | 2025-12-16 |
| `ley-1983-008/` | Ley 8/1983, de 8 de julio, del Consejo de la Cultura Gallega. | 1 | as first published: 21 August 1984 | 2025-12-16 |
| `ley-1984-005/` | Ley 5/1984, de 29 de mayo, de símbolos de Galicia. | 1 | as first published: 24 June 1984 | 2026-05-13 |
| `ley-1984-006/` | Ley 6/1984, de 5 de junio, del Valedor del Pueblo de Galicia. | 7 | as first published, then each change: 3 August 1984 to 4 April 2023 | 2026-10-13 |
| `ley-1985-006/` | Ley 6/1985, de 24 de junio, del Consejo de Cuentas. | 9 | as first published, then each change: 29 July 1985 to 4 April 2023 | 2025-12-16 |
| `ley-1985-009/` | Ley 9/1985, de 30 de julio, de protección de piedras ornamentales. | 3 | as first published, then each change: 6 September 1985 to 9 May 1986 | 2025-12-16 |
| `ley-1985-008/` | Ley 8/1985, de 13 de agosto, de elecciones al Parlamento de Galicia. | 4 | as first published, then each change: 17 August 1985 to 20 September 2015 | 2025-12-16 |
| `ley-1986-003/` | Ley 3/1986, de 18 de diciembre, de Consejos Escolares de Galicia. | 1 | as first published: 27 December 1986 | 2025-12-17 |
| `ley-1987-004/` | Ley 4/1987, de 27 de mayo, de Creación de la Escuela Gallega de Administración Pública. | 3 | as first published, then each change: 22 June 1987 to 30 January 2021 | 2025-12-17 |
| `ley-1987-008/` | Ley 8/1987, de 25 de noviembre, por la que se establece la gratuidad de los estudios de Bachillerato, Formación Profesional y Artes Aplicadas y Oficios Artísticos en los Centros públicos y la autonomía de gestión económica de los Centros docentes públicos no universitarios. | 3 | as first published, then each change: 21 January 1988 to 1 January 2026 | 2026-02-16 |
| `ley-1988-003/` | Ley 3/1988, de 27 de abril, de creación del Instituto Gallego de la Vivienda y Suelo. | 1 | as first published: 30 May 1988 | 2025-12-17 |
| `ley-1988-005/` | Ley 5/1988, de 21 de junio, del uso del gallego como lengua oficial de Galicia por las Entidades locales. | 1 | as first published: 20 July 1988 | 2025-12-17 |
| `ley-1989-013/` | Ley 13/1989, de 10 de octubre, de montes vecinales en mano común. | 10 | as first published, then each change: 9 November 1989 to 1 January 2022 | 2025-12-17 |
| `ley-1989-017/` | Ley 17/1989, de 23 de octubre, de Creación de Escalas del Personal Sanitario al Servicio de la Comunidad Autónoma. | 1 | as first published: 27 October 1989 | 2025-12-17 |
| `ley-1991-013/` | Ley 13/1991, de 9 de diciembre, de tasas, precios y exacciones reguladoras de la Comunidad Autónoma de Galicia. | 2 | as first published, then each change: 14 December 1991 to 12 December 2003 | 2025-12-17 |
| `ley-1992-005/` | Ley 5/1992, de 10 de junio, de creación del Instituto Gallego de Promoción Económica. | 1 | as first published: 27 June 1992 | 2025-12-17 |
| `ley-1992-009/` | Ley 9/1992, de 24 de julio, de educación y promoción de adultos. | 1 | as first published: 7 August 1992 | 2025-12-17 |
| `ley-1993-003/` | Ley 3/1993, de 16 de abril, de las Aparcerías y de los Arrendamientos Rústicos Históricos de Galicia. | 3 | as first published, then each change: 12 May 1993 to 1 January 2011 | 2025-12-17 |
| `ley-1993-009/` | Ley 9/1993, de 8 de julio, de Cofradías de Pescadores de Galicia. | 7 | as first published, then each change: 16 July 1993 to 1 January 2025 | 2025-12-17 |
| `ley-1994-007/` | Ley 7/1994, de 29 de diciembre, por la que se crea el Instituto Lácteo y Ganadero de Galicia. | 3 | as first published, then each change: 6 January 1995 to 1 January 2004 | 2025-12-18 |
| `ley-1995-001/` | Ley 1/1995, de 2 de enero, de protección ambiental de Galicia. | 6 | as first published, then each change: 11 February 1995 to 1 January 2020 | 2025-12-18 |
| `ley-1995-005/` | Ley 5/1995, de 7 de junio, de regulación de las aguas minerales, termales, de manantial y de los establecimientos balnearios de la Comunidad Autónoma de Galicia. | 2 | as first published, then each change: 22 June 1995 to 2 February 2020 | 2025-12-18 |
| `ley-1995-006/` | Ley 6/1995, de 28 de junio, por la que se crea el Consejo Económico y Social de Galicia. | 3 | as first published, then each change: 13 July 1995 to 1 January 2023 | 2025-12-18 |
| `ley-1995-012/` | Ley 12/1995, de 29 de diciembre, del impuesto sobre la Contaminación Atmosférica. | 4 | as first published, then each change: 1 January 1996 to 1 January 2015 | 2025-12-18 |
| `ley-1996-001/` | Ley 1/1996, de 5 de marzo, de regulación de las actividades feriales de Galicia. | 3 | as first published, then each change: 10 April 1996 to 18 January 2011 | 2025-12-18 |
| `ley-1996-002/` | Ley 2/1996, de 8 de mayo, de Galicia, sobre drogas. | 2 | as first published, then each change: 22 July 1996 to 7 March 2026 | 2026-03-09 |
| `ley-1996-006/` | Ley 6/1996, de 9 de julio, de coordinación de los servicios de transportes urbanos e interurbanos por carretera de Galicia. | 3 | as first published, then each change: 19 July 1995 to 1 January 2023 | 2025-12-18 |
| `ley-1996-007/` | Ley 7/1996, de 10 de julio, de desarrollo comarcal. | 2 | as first published, then each change: 20 July 1996 to 6 January 2009 | 2025-12-18 |
| `ley-1996-012/` | Ley 12/1996, de 27 de diciembre, de Creación del Colegio Oficial de Podólogos de Galicia. | 1 | as first published: 21 January 1997 | 2025-12-18 |
| `ley-1997-005/` | Ley 5/1997, de 22 de julio, de Administración Local de Galicia. | 7 | as first published, then each change: 6 November 1997 to 1 January 2016 | 2025-12-18 |
| `ley-1997-008/` | Ley 8/1997, de 20 de agosto, de accesibilidad y supresión de barreras en la Comunidad Autónoma de Galicia. | 2 | as first published, then each change: 29 November 1997 to 17 March 2015 | 2025-12-18 |
| `ley-1998-003/` | Ley 3/1998, de 30 de junio, de Creación del Colegio Oficial de Fisioterapeutas de Galicia. | 1 | as first published: 4 July 1998 | 2025-12-18 |
| `ley-1998-004/` | Ley 4/1998, de 30 de junio, de Creación del Colegio Oficial de Protésicos Dentales de Galicia. | 1 | as first published: 4 July 1998 | 2025-12-18 |
| `ley-1998-005/` | Ley 5/1998, de 18 de diciembre, de Cooperativas de Galicia. | 9 | as first published, then each change: 28 February 1999 to 1 January 2022 | 2026-10-13 |
| `ley-1999-002/` | Ley 2/1999, de 24 de febrero, de Creación del Colegio Profesional de Periodistas de Galicia. | 1 | as first published: 10 March 1999 | 2025-12-18 |
| `ley-1999-003/` | Ley 3/1999, de 11 de marzo, de Creación del Instituto Energético de Galicia. | 1 | as first published: 19 February 1999 | 2025-12-18 |
| `ley-1999-006/` | Ley 6/1999, de 1 de septiembre, del Audiovisual de Galicia. | 3 | as first published, then each change: 9 September 1999 to 1 January 2025 | 2025-12-18 |
| `decreto-legislativo-1999-001/` | Decreto Legislativo 1/1999, de 7 de octubre, por el que se aprueba el texto refundido de la Ley de Régimen Financiero y Presupuestario de Galicia. | 26 | as first published, then each change: 6 November 1999 to 1 January 2026 | 2026-02-16 |
| `ley-2000-005/` | Ley 5/2000, de 28 de diciembre, de Medidas Fiscales y de Régimen Presupuestario y Administrativo. | 4 | oldest version available, then each change: 1 January 2001 to 24 May 2015 | 2025-12-18 |
| `ley-2001-001/` | Ley 1/2001, de 22 de enero, de Creación del Colegio de Educadores Sociales de Galicia. | 1 | as first published: 2 February 2001 | 2025-12-18 |
| `ley-2001-003/` | Ley 3/2001, de 28 de mayo, reguladora del consentimiento informado y de la historia clínica de los pacientes. | 2 | as first published, then each change: 8 July 2001 to 21 May 2005 | 2025-12-18 |
| `ley-2001-004/` | Ley 4/2001, de 31 de mayo, reguladora de la Mediación Familiar. | 2 | as first published, then each change: 18 March 2002 to 8 August 2007 | 2025-12-18 |
| `ley-2001-005/` | Ley 5/2001, de 28 de junio, de Régimen Jurídico de las Concesiones en la isla de Ons. | 2 | as first published, then each change: 11 September 2001 to 1 January 2011 | 2025-12-18 |
| `ley-2001-006/` | Ley 6/2001, de 29 de junio, de adecuación de la normativa de la Comunidad Autónoma de Galicia a la Ley 4/1999, de 13 de enero, de modificación de la Ley 30/1992, de 26 de noviembre, de Régimen Jurídico de las Administraciones Públicas y del Procedimiento Administrativo Común. | 6 | as first published, then each change: 13 July 2001 to 26 October 2017 | 2025-12-18 |
| `ley-2001-011/` | Ley 11/2001, de 18 de septiembre, de Colegios Profesionales de la Comunidad Autónoma de Galicia. | 5 | as first published, then each change: 18 October 2001 to 1 July 2017 | 2025-12-18 |
| `ley-2002-004/` | Ley 4/2002, de 25 de junio, del estatuto de la capitalidad de la ciudad de Santiago de Compostela. | 1 | as first published: 25 July 2002 | 2025-12-18 |
| `ley-2002-008/` | Ley 8/2002, de 18 de diciembre, de protección del ambiente atmosférico de Galicia. | 1 | as first published: 30 January 2003 | 2025-12-18 |
| `ley-2003-006/` | Ley 6/2003, de 9 de diciembre, de tasas, precios y exacciones reguladoras de la Comunidad Autónoma de Galicia. | 27 | as first published, then each change: 12 December 2003 to 1 January 2026 | 2026-02-16 |
| `ley-2003-010/` | Ley 10/2003, de 26 de diciembre, sobre el acceso al entorno de las personas con discapacidad acompañadas de perros de asistencia. | 2 | as first published, then each change: 1 January 2004 to 1 January 2023 | 2025-12-18 |
| `ley-2004-002/` | Ley 2/2004, de 21 de abril, por la que se crea el Servicio de Guardacostas de Galicia. | 4 | as first published, then each change: 13 May 2004 to 26 November 2010 | 2025-12-18 |
| `ley-2004-003/` | Ley 3/2004, de 7 de junio, de creación del Instituto Tecnológico para el Control del Medio Marino de Galicia. | 3 | as first published, then each change: 7 July 2004 to 16 December 2009 | 2025-12-18 |
| `ley-2004-004/` | Ley 4/2004, de 28 de junio, para la aplicación a los municipios de Ferrol, Lugo, Ourense, Pontevedra y Santiago de Compostela del régimen de organización de los municipios de gran población. | 1 | as first published: 8 July 2004 | 2025-12-18 |
| `ley-2004-005/` | Ley 5/2004, de 8 de julio, de Cámaras Oficiales de Comercio, Industria y Navegación de Galicia. | 6 | as first published, then each change: 10 August 2004 to 1 January 2024 | 2025-12-18 |
| `ley-2004-011/` | Ley 11/2004, de 19 de noviembre, de inspección de consumo de Galicia. | 2 | as first published, then each change: 22 December 2004 to 1 January 2023 | 2025-12-18 |
| `decreto-legislativo-2005-001/` | Decreto Legislativo 1/2005, de 10 de marzo, por el que se aprueba el texto refundido de las leyes 7/1985, de 17 de julio, y 4/1996, de 31 de mayo, de cajas de ahorros de Galicia. | 5 | oldest version available, then each change: 28 May 2005 to 3 February 2015 | 2023-12-26 |
| `ley-2005-005/` | Ley 5/2005, de 25 de abril, reguladora del recurso de casación en materia de derecho civil de Galicia. | 1 | as first published: 19 May 2005 | 2025-12-18 |
| `ley-2006-001/` | Ley 1/2006, de 5 de junio, del Consejo Agrario Gallego. | 2 | as first published, then each change: 15 June 2006 to 1 January 2024 | 2025-12-18 |
| `ley-2006-002/` | Ley 2/2006, de 14 de junio, de derecho civil de Galicia. | 5 | as first published, then each change: 19 July 2006 to 20 December 2017 | 2025-12-18 |
| `ley-2006-003/` | Ley 3/2006, de 30 de junio, de creación del Colegio Profesional de Logopedas de Galicia. | 4 | as first published, then each change: 2 August 2006 to 3 May 2011 | 2025-12-18 |
| `ley-2006-005/` | Ley 5/2006, de 30 de junio, para la protección, la conservación y la mejora de los ríos gallegos. | 1 | as first published: 18 July 2006 | 2025-12-18 |
| `ley-2006-008/` | Ley 8/2006, de 1 de diciembre, de creación del Colegio Profesional de Ingeniería Técnica en Informática de Galicia. | 5 | as first published, then each change: 2 January 2007 to 1 July 2017 | 2025-12-19 |
| `ley-2006-009/` | Ley 9/2006, de 1 de diciembre, de creación del Colegio Profesional de Joyería, Orfebrería, Platería, Relojería y Gemología de Galicia | 5 | as first published, then each change: 3 January 2007 to 1 July 2017 | 2025-12-19 |
| `ley-2006-010/` | Ley 10/2006, de 1 de diciembre, de creación del Colegio Profesional de Ingeniería en Informática de Galicia. | 5 | as first published, then each change: 4 January 2007 to 1 July 2017 | 2025-12-19 |
| `ley-2006-011/` | Ley 11/2006, de 1 de diciembre, de creación del Colegio Profesional de Higienistas Dentales de Galicia. | 4 | as first published, then each change: 7 January 2007 to 3 May 2011 | 2025-12-19 |
| `ley-2006-012/` | Ley 12/2006, de 1 de diciembre, de fundaciones de interés gallego. | 2 | as first published, then each change: 19 January 2007 to 1 January 2011 | 2025-12-19 |
| `ley-2006-013/` | Ley 13/2006, de 27 de diciembre, de horarios comerciales de Galicia. | 2 | as first published, then each change: 29 December 2006 to 15 February 2013 | 2026-04-22 |
| `ley-2006-017/` | Ley 17/2006, de 27 de diciembre, del libro y de la lectura de Galicia. | 2 | as first published, then each change: 30 January 2007 to 24 February 2010 | 2025-12-19 |
| `ley-2007-001/` | Ley 1/2007, de 15 de enero, de la Academia Gallega de Seguridad Pública. | 3 | as first published, then each change: 24 January 2007 to 30 January 2021 | 2025-12-19 |
| `ley-2007-003/` | Ley 3/2007, de 9 de abril, de prevención y defensa contra los incendios forestales de Galicia. | 13 | as first published, then each change: 18 April 2007 to 1 January 2026 | 2026-02-16 |
| `ley-2007-004/` | Ley 4/2007, de 20 de abril, de coordinación de policías locales. | 4 | as first published, then each change: 23 May 2007 to 1 January 2026 | 2026-02-16 |
| `ley-2007-005/` | Ley 5/2007, de 7 de mayo, de emergencias de Galicia. | 4 | as first published, then each change: 5 June 2007 to 30 January 2021 | 2025-12-19 |
| `ley-2007-008/` | Ley 8/2007, de 13 de junio, de Policía de Galicia. | 1 | as first published: 12 July 2007 | 2025-12-19 |
| `ley-2007-009/` | Ley 9/2007, de 13 de junio, de subvenciones de Galicia. | 7 | as first published, then each change: 25 September 2007 to 1 January 2024 | 2026-06-26 |
| `ley-2007-011/` | Ley 11/2007, de 27 de julio, gallega para la prevención y el tratamiento integral de la violencia de género. | 6 | as first published, then each change: 8 August 2007 to 1 January 2023 | 2025-12-19 |
| `ley-2007-014/` | Ley 14/2007, de 30 de octubre, por la que se crea y regula el Instituto Gallego de Seguridad y Salud Laboral. | 6 | as first published, then each change: 15 November 2007 to 1 January 2019 | 2025-12-19 |
| `ley-2007-015/` | Ley 15/2007, de 13 de diciembre, de creación del Colegio Oficial de Ingenieras e Ingenieros Químicos de Galicia. | 4 | as first published, then each change: 13 January 2008 to 3 May 2011 | 2025-12-19 |
| `decreto-legislativo-2008-001/` | Decreto Legislativo 1/2008, de 13 de marzo, por el que se aprueba el texto refundido de la Ley de la función pública de Galicia. | 5 | as first published, then each change: 14 June 2008 to 24 May 2015 | 2026-04-22 |
| `ley-2008-001/` | Ley 1/2008, de 17 de abril, de creación del Colegio Profesional de Detectives Privados y Privadas de Galicia. | 5 | as first published, then each change: 18 May 2008 to 1 July 2017 | 2025-12-19 |
| `ley-2008-002/` | Ley 2/2008, de 6 de mayo, por la que se desarrolla la libre prestación de servicios de transporte marítimo de personas en aguas interiores de Galicia. | 1 | as first published: 12 August 2008 | 2025-12-19 |
| `ley-2008-003/` | Ley 3/2008, de 23 de mayo, de ordenación de la minería de Galicia. | 13 | as first published, then each change: 26 June 2008 to 1 January 2026 | 2026-02-16 |
| `ley-2008-004/` | Ley 4/2008, de 23 de mayo, de creación de la Agencia Gallega de las Industrias Culturales. | 1 | as first published: 11 June 2008 | 2025-12-19 |
| `ley-2008-005/` | Ley 5/2008, de 23 de mayo, por la que se regula el Consejo Gallego de Relaciones Laborales. | 1 | as first published: 1 July 2008 | 2025-12-19 |
| `ley-2008-007/` | Ley 7/2008, de 7 de julio, de protección del paisaje de Galicia. | 6 | as first published, then each change: 18 August 2008 to 1 January 2026 | 2026-02-16 |
| `ley-2008-008/` | Ley 8/2008, de 10 de julio, de salud de Galicia. | 19 | as first published, then each change: 24 September 2008 to 8 April 2026 | 2026-05-04 |
| `ley-2008-011/` | Ley 11/2008, de 3 de diciembre, de pesca de Galicia. | 8 | oldest version available, then each change: 16 June 2009 to 1 January 2024 | 2025-12-19 |
| `ley-2008-013/` | Ley 13/2008, de 3 de diciembre, de servicios sociales de Galicia. | 19 | as first published, then each change: 18 March 2009 to 27 March 2026 | 2026-06-26 |
| `ley-2008-015/` | Ley 15/2008, de 19 de diciembre, del impuesto sobre el daño medioambiental causado por determinados usos y aprovechamientos del agua embalsada. | 3 | as first published, then each change: 30 December 2008 to 1 January 2020 | 2025-12-19 |
| `ley-2008-017/` | Ley 17/2008, de 29 de diciembre, de participación institucional de las organizaciones sindicales y empresariales más representativas de Galicia. | 1 | as first published: 20 January 2009 | 2025-12-19 |
| `ley-2009-005/` | Ley 5/2009, de 26 de noviembre, de medidas urgentes para la modernización del sector del transporte público de Galicia. | 2 | as first published, then each change: 30 November 2009 to 23 July 2016 | 2025-12-19 |
| `ley-2009-008/` | Ley 8/2009, de 22 de diciembre, por la que se regula el aprovechamiento eólico en Galicia y se crean el canon eólico y el Fondo de Compensación Ambiental. | 19 | as first published, then each change: 30 December 2009 to 1 January 2027 | 2026-03-27 |
| `ley-2010-004/` | Ley 4/2010, de 23 de junio, de fomento del sector naval de Galicia. | 1 | as first published: 6 July 2010 | 2026-05-26 |
| `ley-2010-005/` | Ley 5/2010, de 23 de junio, por la que se establece y regula una red de apoyo a la mujer embarazada. | 1 | as first published: 7 July 2010 | 2025-12-19 |
| `ley-2010-009/` | Ley 9/2010, de 4 de noviembre, de aguas de Galicia. | 18 | as first published, then each change: 18 December 2010 to 1 January 2026 | 2026-02-16 |
| `ley-2010-013/` | Ley 13/2010, de 17 de diciembre, del comercio interior de Galicia. | 12 | as first published, then each change: 18 January 2011 to 1 January 2026 | 2026-02-16 |
| `ley-2010-016/` | Ley 16/2010, de 17 de diciembre, de organización y funcionamiento de la Administración general y del sector público autonómico de Galicia. | 15 | as first published, then each change: 1 January 2011 to 1 January 2026 | 2026-02-16 |
| `ley-2010-012/` | Ley 12/2010, de 22 de diciembre, de racionalización del gasto en la prestación farmacéutica de la Comunidad Autónoma de Galicia. | 3 | as first published, then each change: 29 December 2010 to 5 July 2011 | 2025-12-19 |
| `ley-2010-015/` | Ley 15/2010, de 28 de diciembre, de medidas fiscales y administrativas. | 4 | as first published, then each change: 1 January 2011 to 20 May 2015 | 2025-12-19 |
| `ley-2011-002/` | Ley 2/2011, de 16 de junio, de disciplina presupuestaria y sostenibilidad financiera. | 3 | as first published, then each change: 30 June 2011 to 10 February 2017 | 2025-12-19 |
| `ley-2011-003/` | Ley 3/2011, de 30 de junio, de apoyo a la familia y a la convivencia de Galicia. | 2 | as first published, then each change: 13 September 2011 to 10 February 2021 | 2025-12-19 |
| `ley-2011-004/` | Ley 4/2011, de 30 de junio, de convivencia y participación de la comunidad educativa. | 2 | as first published, then each change: 16 July 2011 to 1 January 2026 | 2026-02-16 |
| `decreto-legislativo-2011-001/` | Decreto Legislativo 1/2011, de 28 de julio, por el que se aprueba el texto refundido de las disposiciones legales de la Comunidad Autónoma de Galicia en materia de tributos cedidos por el Estado. | 28 | as first published, then each change: 21 October 2011 to 27 March 2026 | 2026-05-04 |
| `ley-2011-005/` | Ley 5/2011, de 30 de septiembre, del patrimonio de la Comunidad Autónoma de Galicia. | 6 | as first published, then each change: 24 November 2011 to 3 December 2023 | 2025-12-19 |
| `ley-2011-007/` | Ley 7/2011, de 27 de octubre, del Turismo de Galicia. | 6 | as first published, then each change: 11 December 2011 to 1 January 2020 | 2025-12-19 |
| `ley-2011-010/` | Ley 10/2011, de 28 de noviembre, de Acción Voluntaria. | 2 | as first published, then each change: 22 December 2011 to 1 January 2018 | 2025-12-19 |
| `ley-2012-001/` | Ley 1/2012, de 29 de febrero, de medidas temporales en determinadas materias del empleo público de la Comunidad Autónoma de Galicia. | 5 | as first published, then each change: 3 March 2012 to 1 January 2019 | 2025-12-19 |
| `ley-2012-002/` | Ley 2/2012, de 28 de marzo, gallega de protección general de las personas consumidoras y usuarias. | 9 | as first published, then each change: 1 May 2012 to 1 January 2026 | 2026-02-16 |
| `ley-2012-003/` | Ley 3/2012, de 2 de abril, del deporte de Galicia. | 7 | as first published, then each change: 14 April 2012 to 19 December 2025 | 2026-02-17 |
| `ley-2012-004/` | Ley 4/2012, de 12 de abril, del Área Metropolitana de Vigo. | 2 | as first published, then each change: 23 May 2012 to 1 September 2016 | 2025-12-19 |
| `ley-2012-005/` | Ley 5/2012, de 15 de junio, de bibliotecas de Galicia. | 1 | as first published: 17 July 2012 | 2025-12-19 |
| `ley-2012-006/` | Ley 6/2012, de 19 de junio, de juventud de Galicia. | 5 | as first published, then each change: 9 August 2012 to 1 January 2025 | 2025-12-19 |
| `ley-2012-007/` | Ley 7/2012, de 28 de junio, de montes de Galicia. | 15 | as first published, then each change: 12 August 2012 to 1 January 2026 | 2026-06-26 |
| `ley-2012-008/` | Ley 8/2012, de 29 de junio, de vivienda de Galicia. | 12 | as first published, then each change: 13 August 2012 to 1 January 2026 | 2026-02-16 |
| `ley-2012-009/` | Ley 9/2012, de 3 de agosto, de adaptación de las disposiciones básicas del Real Decreto-ley 20/2012, de 13 de julio, de medidas para garantizar la estabilidad presupuestaria y de fomento de la competitividad, en materia de empleo público. | 2 | as first published, then each change: 10 August 2012 to 24 May 2015 | 2025-12-19 |
| `ley-2013-003/` | Ley 3/2013, de 20 de mayo, de impulso y ordenación de las infraestructuras de telecomunicaciones de Galicia. | 5 | as first published, then each change: 7 July 2013 to 1 January 2025 | 2025-12-19 |
| `ley-2013-004/` | Ley 4/2013, de 30 de mayo, de transporte público de personas en vehículos de turismo de Galicia. | 8 | as first published, then each change: 14 July 2013 to 1 January 2026 | 2026-02-16 |
| `ley-2013-005/` | Ley 5/2013, de 30 de mayo, de fomento de la investigación y de la innovación de Galicia. | 6 | as first published, then each change: 17 September 2013 to 1 January 2025 | 2025-12-19 |
| `ley-2013-006/` | Ley 6/2013, de 13 de junio, del Sistema universitario de Galicia. | 5 | as first published, then each change: 4 July 2013 to 1 January 2025 | 2025-12-19 |
| `ley-2013-007/` | Ley 7/2013, de 13 de junio, de la galleguidad. | 2 | as first published, then each change: 5 July 2013 to 16 August 2016 | 2025-12-19 |
| `ley-2013-008/` | Ley 8/2013, de 28 de junio, de carreteras de Galicia. | 12 | as first published, then each change: 12 October 2013 to 1 January 2026 | 2026-02-16 |
| `ley-2013-010/` | Ley 10/2013, de 27 de noviembre, de inclusión social de Galicia. | 4 | as first published, then each change: 1 January 2014 to 1 January 2023 | 2025-12-19 |
| `ley-2013-012/` | Ley 12/2013, de 9 de diciembre, de garantías de prestaciones sanitarias. | 2 | as first published, then each change: 3 March 2014 to 27 January 2015 | 2025-12-19 |
| `ley-2013-009/` | Ley 9/2013, de 19 de diciembre, del emprendimiento y de la competitividad económica de Galicia. | 8 | as first published, then each change: 28 December 2013 to 1 January 2026 | 2026-02-16 |
| `ley-2013-013/` | Ley 13/2013, de 23 de diciembre, de caza de Galicia. | 9 | as first published, then each change: 28 January 2014 to 1 January 2026 | 2026-02-16 |
| `ley-2013-014/` | Ley 14/2013, de 26 de diciembre, de racionalización del sector público autonómico. | 12 | as first published, then each change: 16 February 2014 to 1 January 2026 | 2026-02-16 |
| `ley-2014-001/` | Ley 1/2014, de 24 de marzo, para el aprovechamiento de la lengua portuguesa y vínculos con la lusofonía. | 1 | as first published: 9 April 2014 | 2025-12-19 |
| `ley-2014-002/` | Ley 2/2014, de 14 de abril, por la igualdad de trato y la no discriminación de lesbianas, gays, transexuales, bisexuales e intersexuales en Galicia. | 1 | as first published: 26 April 2014 | 2025-12-19 |
| `ley-2014-003/` | Ley 3/2014, de 24 de abril, del Consejo Consultivo de Galicia. | 5 | as first published, then each change: 29 April 2014 to 4 April 2023 | 2025-12-19 |
| `ley-2014-005/` | Ley 5/2014, de 27 de mayo, de medidas urgentes derivadas de la entrada en vigor de la Ley 27/2013, de 27 de diciembre, de racionalización y sostenibilidad de la Administración local. | 1 | as first published: 31 May 2014 | 2025-12-19 |
| `ley-2014-007/` | Ley 7/2014, de 26 de septiembre, de archivos y documentos de Galicia. | 2 | as first published, then each change: 27 October 2014 to 15 August 2019 | 2025-12-19 |
| `ley-2014-010/` | Ley 10/2014, de 3 de diciembre, de accesibilidad. | 2 | as first published, then each change: 17 March 2015 to 30 January 2021 | 2025-12-19 |
| `ley-2014-012/` | Ley 12/2014, de 22 de diciembre, de medidas fiscales y administrativas. | 5 | as first published, then each change: 1 January 2015 to 9 October 2019 | 2025-12-19 |
| `decreto-legislativo-2015-001/` | Decreto Legislativo 1/2015, de 12 de febrero, por el que se aprueba el texto refundido de las disposiciones legales de la Comunidad Autónoma de Galicia en materia de política industrial. | 8 | oldest version available, then each change: 10 July 2015 to 1 January 2026 | 2026-02-16 |
| `ley-2015-001/` | Ley 1/2015, de 1 de abril, de garantía de la calidad de los servicios públicos y de la buena administración. | 1 | as first published: 20 May 2015 | 2025-12-19 |
| `ley-2015-002/` | Ley 2/2015, de 29 de abril, del empleo público de Galicia. | 15 | as first published, then each change: 24 May 2015 to 1 January 2026 | 2026-02-17 |
| `ley-2015-003/` | Ley 3/2015, de 12 de junio, de creación del Colegio Oficial de Dietistas-Nutricionistas de Galicia. | 1 | as first published: 28 July 2015 | 2025-12-19 |
| `ley-2015-004/` | Ley 4/2015, de 17 de junio, de mejora de la estructura territorial agraria de Galicia. | 10 | as first published, then each change: 3 August 2015 to 1 January 2025 | 2026-04-27 |
| `ley-2015-005/` | Ley 5/2015, de 26 de junio, de derechos y garantías de la dignidad de las personas enfermas terminales. | 1 | as first published: 16 August 2015 | 2025-12-19 |
| `ley-2015-007/` | Ley 7/2015, de 7 de agosto, de iniciativa legislativa popular y participación ciudadana en el Parlamento de Galicia. | 1 | as first published: 20 August 2015 | 2025-12-19 |
| `ley-2015-009/` | Ley 9/2015, de 7 de agosto, de financiación de las formaciones políticas y de las fundaciones y entidades vinculadas o dependientes de ellas. | 1 | as first published: 20 September 2015 | 2025-12-19 |
| `ley-2015-013/` | Ley 13/2015, de 24 de diciembre, de medidas fiscales y administrativas. | 3 | as first published, then each change: 1 January 2016 to 10 March 2017 | 2025-12-19 |
| `ley-2016-001/` | Ley 1/2016, de 18 de enero, de transparencia y buen gobierno. | 6 | as first published, then each change: 6 March 2016 to 1 May 2026 | 2026-05-04 |
| `ley-2016-002/` | Ley 2/2016, de 10 de febrero, del suelo de Galicia. | 15 | as first published, then each change: 19 March 2016 to 1 January 2026 | 2026-02-16 |
| `ley-2016-003/` | Ley 3/2016, de 1 de marzo, de medidas en materia de proyectos públicos de urgencia o de excepcional interés. | 1 | as first published: 20 March 2016 | 2025-12-19 |
| `ley-2016-004/` | Ley 4/2016, de 4 de abril, de ordenación de la asistencia jurídica de la Administración General de la Comunidad Autónoma de Galicia y de su sector público. | 5 | as first published, then each change: 13 April 2016 to 1 January 2025 | 2025-12-19 |
| `ley-2016-005/` | Ley 5/2016, de 4 de mayo, del patrimonio cultural de Galicia. | 11 | as first published, then each change: 16 August 2016 to 1 January 2026 | 2026-02-20 |
| `ley-2016-006/` | Ley 6/2016, de 4 de mayo, de la economía social de Galicia. | 1 | as first published: 7 June 2016 | 2025-12-19 |
| `ley-2016-010/` | Ley 10/2016, de 19 de julio, de medidas urgentes para la actualización del sistema de transporte público de Galicia. | 1 | as first published: 23 July 2016 | 2025-12-19 |
| `ley-2016-011/` | Ley 11/2016, de 19 de julio, de creación de los colegios provinciales de economistas por fusión de los colegios de titulares mercantiles y de economistas existentes en la Comunidad Autónoma de Galicia. | 1 | as first published: 27 July 2016 | 2025-12-19 |
| `ley-2016-013/` | Ley 13/2016, de 26 de julio, de creación del Colegio Oficial de Terapeutas Ocupacionales de Galicia. | 1 | as first published: 18 August 2016 | 2025-12-19 |
| `ley-2016-015/` | Ley 15/2016, de 28 de julio, del Plan gallego de estadística 2017-2021. | 2 | as first published, then each change: 1 January 2017 to 1 January 2022 | 2026-06-24 |
| `ley-2017-002/` | Ley 2/2017, de 8 de febrero, de medidas fiscales, administrativas y de ordenación. | 7 | as first published, then each change: 1 January 2017 to 1 January 2025 | 2026-02-19 |
| `ley-2017-004/` | Ley 4/2017, de 3 de octubre, de protección y bienestar de los animales de compañía en Galicia. | 4 | as first published, then each change: 11 January 2018 to 1 January 2025 | 2025-12-19 |
| `ley-2017-005/` | Ley 5/2017, de 19 de octubre, de fomento de la implantación de iniciativas empresariales en Galicia. | 10 | as first published, then each change: 26 October 2017 to 1 January 2024 | 2025-12-19 |
| `ley-2017-006/` | Ley 6/2017, de 12 de diciembre, de puertos de Galicia. | 10 | as first published, then each change: 14 June 2018 to 1 January 2025 | 2026-05-26 |
| `ley-2017-007/` | Ley 7/2017, de 14 de diciembre, de medidas de la eficiencia energética y garantía de accesibilidad a la energía eléctrica. | 3 | as first published, then each change: 1 January 2018 to 1 January 2024 | 2025-12-20 |
| `ley-2017-010/` | Ley 10/2017, de 27 de diciembre, de espectáculos públicos y actividades recreativas de Galicia. | 2 | as first published, then each change: 2 July 2018 to 1 January 2026 | 2026-02-16 |
| `ley-2018-003/` | Ley 3/2018, de 26 de diciembre, de medidas fiscales y administrativas. | 2 | as first published, then each change: 1 January 2019 to 1 January 2025 | 2025-12-20 |
| `ley-2019-001/` | Ley 1/2019, de 22 de abril, de rehabilitación y de regeneración y renovación urbanas de Galicia. | 4 | as first published, then each change: 22 May 2019 to 1 January 2026 | 2026-02-16 |
| `ley-2019-003/` | Ley 3/2019, de 2 de julio, de ordenación farmacéutica de Galicia. | 3 | as first published, then each change: 30 July 2019 to 1 January 2026 | 2026-02-16 |
| `ley-2019-004/` | Ley 4/2019, de 17 de julio, de administración digital de Galicia. | 4 | as first published, then each change: 15 August 2019 to 1 January 2026 | 2026-02-16 |
| `ley-2019-005/` | Ley 5/2019, de 2 de agosto, del patrimonio natural y de la biodiversidad de Galicia. | 6 | as first published, then each change: 27 August 2019 to 1 January 2025 | 2026-04-17 |
| `ley-2019-009/` | Ley 9/2019, de 11 de diciembre, de medidas de garantía del abastecimiento en episodios de sequía y en situaciones de riesgo sanitario. | 1 | as first published: 11 January 2020 | 2025-12-20 |
| `ley-2019-008/` | Ley 8/2019, de 23 de diciembre, de regulación del aprovechamiento lúdico de las aguas termales de Galicia. | 1 | as first published: 2 February 2020 | 2025-12-20 |
| `ley-2021-001/` | Ley 1/2021, de 8 de enero, de ordenación del territorio de Galicia. | 4 | as first published, then each change: 14 February 2021 to 1 January 2026 | 2026-02-16 |
| `ley-2021-002/` | Ley 2/2021, de 8 de enero, de pesca continental de Galicia. | 4 | as first published, then each change: 4 February 2021 to 1 January 2026 | 2026-02-16 |
| `ley-2021-005/` | Ley 5/2021, de 2 de febrero, de impulso demográfico de Galicia. | 2 | as first published, then each change: 10 February 2021 to 1 January 2026 | 2026-02-16 |
| `ley-2021-006/` | Ley 6/2021, de 17 de febrero, de residuos y suelos contaminados de Galicia. | 3 | as first published, then each change: 17 March 2021 to 1 January 2023 | 2025-12-20 |
| `ley-2021-007/` | Ley 7/2021, de 17 de febrero, de museos y otros centros museísticos de Galicia. | 1 | as first published: 17 March 2021 | 2025-12-20 |
| `ley-2021-009/` | Ley 9/2021, de 25 de febrero, de simplificación administrativa y de apoyo a la reactivación económica de Galicia. | 8 | as first published, then each change: 18 March 2021 to 1 January 2026 | 2026-02-16 |
| `ley-2021-010/` | Ley 10/2021, de 9 de marzo, reguladora de la acción exterior y de la cooperación para el desarrollo de Galicia. | 1 | as first published: 4 April 2021 | 2025-12-20 |
| `ley-2021-011/` | Ley 11/2021, de 14 de mayo, de recuperación de la tierra agraria de Galicia. | 6 | as first published, then each change: 22 May 2021 to 1 January 2026 | 2026-02-17 |
| `ley-2021-012/` | Ley 12/2021, de 15 de julio, de reconocimiento de la universidad privada Universidad Intercontinental de la Empresa, con sede en la Comunidad Autónoma de Galicia. | 1 | as first published: 22 July 2021 | 2025-12-20 |
| `ley-2021-016/` | Ley 16/2021, de 20 de diciembre, del Plan gallego de estadística 2022-2026. | 1 | as first published: 1 January 2022 | 2026-06-24 |
| `ley-2022-001/` | Ley 1/2022, de 12 de julio, de mejora de la gestión del ciclo integral del agua. | 2 | as first published, then each change: 1 September 2022 to 1 January 2026 | 2026-02-16 |
| `ley-2022-003/` | Ley 3/2022, de 18 de octubre, de áreas empresariales de Galicia. | 5 | as first published, then each change: 10 November 2022 to 1 January 2026 | 2026-02-17 |
| `ley-2023-003/` | Ley 3/2023, de 4 de julio, reguladora de los juegos de Galicia. | 4 | as first published, then each change: 6 October 2023 to 1 January 2026 | 2026-02-16 |
| `ley-2023-004/` | Ley 4/2023, de 6 de julio, de ordenación y gestión integrada del litoral de Galicia. | 4 | as first published, then each change: 2 August 2023 to 30 May 2024 | 2025-12-20 |
| `ley-2023-006/` | Ley 6/2023, de 2 de noviembre, del patrimonio de la Comunidad Autónoma de Galicia. | 3 | as first published, then each change: 3 December 2023 to 1 January 2026 | 2026-02-16 |
| `ley-2023-007/` | Ley 7/2023, de 30 de noviembre, para la igualdad efectiva de mujeres y hombres de Galicia. | 2 | as first published, then each change: 31 December 2023 to 1 January 2025 | 2025-12-20 |
| `ley-2023-008/` | Ley 8/2023, de 14 de diciembre, de artesanía de Galicia. | 1 | as first published: 8 January 2024 | 2025-12-20 |
| `ley-2024-001/` | Ley 1/2024, de 11 de enero, de la calidad alimentaria de Galicia. | 3 | as first published, then each change: 7 February 2024 to 1 January 2026 | 2026-02-16 |
| `ley-2024-002/` | Ley 2/2024, de 7 de noviembre, de promoción de los beneficios sociales y económicos de los proyectos que utilizan los recursos naturales de Galicia. | 3 | as first published, then each change: 12 November 2024 to 1 January 2026 | 2026-02-16 |
| `ley-2024-003/` | Ley 3/2024, de 5 de diciembre, de cultura inclusiva y accesible de Galicia. | 2 | as first published, then each change: 31 December 2024 to 1 January 2026 | 2026-02-16 |
| `ley-2024-005/` | Ley 5/2024, de 27 de diciembre, de medidas fiscales y administrativas. | 4 | oldest version available, then each change: 1 January 2025 to 27 March 2026 | 2026-03-27 |
| `ley-2024-006/` | Ley 6/2024, de 27 de diciembre, de estadística de Galicia. | 2 | as first published, then each change: 28 January 2025 to 1 January 2026 | 2026-02-16 |
| `ley-2025-001/` | Ley 1/2025, de 14 de marzo, de servicios de los medios públicos de comunicación audiovisual de Galicia para la sociedad digital. | 1 | as first published: 7 April 2025 | 2025-12-20 |
| `ley-2025-005/` | Ley 5/2025, de 23 de diciembre, de medidas fiscales y administrativas. | 1 | as first published: 1 January 2026 | 2026-04-29 |
| `ley-2025-006/` | Ley 6/2025, de 23 de diciembre, de protección de la salud de las personas menores y prevención de las conductas adictivas. | 1 | as first published: 7 March 2026 | 2026-02-19 |
| `ley-2026-001/` | Ley 1/2026, de 5 de febrero, del clima de Galicia. | 1 | as first published: 3 March 2026 | 2026-03-11 |
| `ley-1983-011/` | Ley 11/1983, de 29 de diciembre, de Actuación Intensiva en las Parroquias Rurales. | 2 | as first published, then each change: 22 February 1984 to 3 August 2015; **repealed** 3 August 2015 by Ley 4/2015, de 17 de junio (BOE-A-2015-9230) | 2025-12-16 |
| `ley-1985-010/` | Ley 10/1985, de 14 de agosto, de Concentración Parcelaria para Galicia. | 7 | as first published, then each change: 23 August 1985 to 3 August 2015; **repealed** 3 August 2015 by Ley 4/2015, de 17 de junio (BOE-A-2015-9230) | 2025-12-16 |
| `ley-1985-014/` | Ley 14/1985, de 23 de octubre, reguladora de los Juegos y Apuestas en Galicia. | 12 | as first published, then each change: 21 November 1985 to 6 October 2023; **repealed** 6 October 2023 by Ley 3/2023, de 4 de julio (BOE-A-2023-19355) | 2025-12-17 |
| `ley-1988-001/` | Ley 1/1988, de 19 de enero, de iniciativa legislativa popular ante el Parlamento de Galicia. | 3 | as first published, then each change: 27 January 1988 to 20 August 2015; **repealed** 20 August 2015 by Ley 7/2015, de 7 de agosto (BOE-A-2015-10202) | 2025-12-17 |
| `ley-1988-009/` | Ley 9/1988, de 19 de julio, de Estadística de Galicia. | 6 | as first published, then each change: 23 August 1988 to 28 January 2025; **repealed** 28 January 2025 by Ley 6/2024, de 27 de diciembre (BOE-A-2025-2146) | 2025-12-17 |
| `ley-1992-001/` | Ley 1/1992, de 11 de marzo, de Artesanía de Galicia. | 3 | as first published, then each change: 12 April 1992 to 8 January 2024; **repealed** 8 January 2024 by Ley 8/2023, de 14 de diciembre (BOE-A-2024-2664) | 2025-12-17 |
| `ley-1992-007/` | Ley 7/1992, de 24 de julio, de Pesca Fluvial. | 4 | as first published, then each change: 5 November 1992 to 4 February 2021; **repealed** 4 February 2021 by Ley 2/2021, de 8 de enero (BOE-A-2021-4520) | 2025-12-17 |
| `ley-1992-013/` | Ley 13/1992, de 9 de noviembre, sobre la revisión del Mapa sanitario para crear el área de salud del Salnés. | 2 | as first published, then each change: 6 December 1992 to 29 April 2018; **repealed** 29 April 2018 by Ley 1/2018, de 2 de abril (BOE-A-2018-5392) | 2025-12-17 |
| `ley-1993-001/` | Ley 1/1993, de 13 de abril, de Protección de Animales Domésticos y Salvajes en Cautividad. | 4 | as first published, then each change: 23 April 1993 to 11 January 2018; **repealed** 11 January 2018 by Ley 4/2017, de 3 de octubre (BOE-A-2017-12357) | 2025-12-17 |
| `ley-1995-008/` | Ley 8/1995, de 30 de octubre, del patrimonio cultural de Galicia. | 7 | as first published, then each change: 9 November 1995 to 16 August 2016; **repealed** 16 August 2016 by Ley 5/2016, de 4 de mayo (BOE-A-2016-5942) | 2025-12-18 |
| `ley-1995-010/` | Ley 10/1995, de 23 de noviembre, de ordenación del territorio de Galicia. | 8 | as first published, then each change: 25 December 1995 to 14 February 2021; **repealed** 14 February 2021 by Ley 1/2021, de 8 de enero (BOE-A-2021-4519) | 2025-12-18 |
| `ley-1999-005/` | Ley 5/1999, de 21 de mayo, de ordenación farmacéutica. | 7 | as first published, then each change: 26 June 1999 to 30 July 2019; **repealed** 30 July 2019 by Ley 3/2019, de 2 de julio (BOE-A-2019-13517) | 2025-12-18 |
| `ley-2001-009/` | Ley 9/2001, de 21 de agosto, de Conservación de la Naturaleza. | 3 | as first published, then each change: 5 September 2001 to 27 August 2019; **repealed** 27 August 2019 by Ley 5/2019, de 2 de agosto (BOE-A-2019-13519) | 2026-10-27 |
| `ley-2002-009/` | Ley 9/2002, de 30 de diciembre, de Ordenación Urbanística y Protección del Medio Rural de Galicia. | 15 | as first published, then each change: 1 January 2003 to 19 March 2016; **repealed** 19 March 2016 by Ley 2/2016, de 10 de febrero (BOE-A-2016-3191) | 2025-12-18 |
| `ley-2003-003/` | Ley 3/2003, de 19 de junio, de cooperación para el desarrollo. | 4 | as first published, then each change: 4 July 2003 to 4 April 2021; **repealed** 4 April 2021 by Ley 10/2021, de 9 de marzo (BOE-A-2021-5211) | 2025-12-18 |
| `ley-2003-007/` | Ley 7/2003, de 9 de diciembre, de ordenación sanitaria de Galicia. | 4 | as first published, then each change: 19 February 2004 to 24 September 2008; **repealed** 24 September 2008 by Ley 8/2008, de 10 de julio (BOE-A-2008-14134) | 2025-12-18 |
| `ley-2004-007/` | Ley 7/2004, de 16 de julio, gallega para la igualdad de mujeres y hombres. | 8 | as first published, then each change: 23 August 2004 to 18 February 2016; **repealed** 18 February 2016 by Decreto Legislativo 2/2015, de 12 de febrero (DOG-g-2015-90667) | 2025-12-18 |
| `ley-2005-002/` | Ley 2/2005, de 18 de febrero, de promoción y defensa de la calidad alimentaria gallega. | 6 | as first published, then each change: 12 March 2005 to 7 February 2024; **repealed** 7 February 2024 by Ley 1/2024, de 11 de enero (BOE-A-2024-2778) | 2025-12-18 |
| `ley-2006-004/` | Ley 4/2006, de 30 de junio, de transparencia y de buenas prácticas en la Administración pública gallega. | 5 | as first published, then each change: 3 August 2006 to 6 March 2016; **repealed** 6 March 2016 by Ley 1/2016, de 18 de enero (BOE-A-2016-3190) | 2026-08-21 |
| `ley-2007-006/` | Ley 6/2007, de 11 de mayo, de Medidas urgentes en materia de ordenación del territorio y del litoral de Galicia. | 6 | as first published, then each change: 17 May 2007 to 14 February 2021; **repealed** 14 February 2021 by Ley 1/2021, de 8 de enero (BOE-A-2021-4519) | 2025-12-19 |
| `ley-2008-010/` | Ley 10/2008, de 3 de noviembre, de residuos de Galicia. | 4 | as first published, then each change: 19 February 2009 to 17 March 2021; **repealed** 17 March 2021 by Ley 6/2021, de 17 de febrero (BOE-A-2021-5137) | 2025-12-19 |
| `ley-2010-011/` | Ley 11/2010, de 17 de diciembre, de prevención del consumo de bebidas alcohólicas en menores de edad. | 2 | as first published, then each change: 28 February 2011 to 7 March 2026; **repealed** 7 March 2026 by Ley 6/2025, de 23 de diciembre (BOE-A-2026-3386) | 2026-03-06 |
| `ley-2011-006/` | Ley 6/2011, de 13 de octubre, de movilidad de tierras. | 8 | as first published, then each change: 15 November 2011 to 22 May 2021; **repealed** 22 May 2021 by Ley 11/2021, de 14 de mayo (BOE-A-2021-10669) | 2025-12-19 |
| `ley-2011-009/` | Ley 9/2011, de 9 de noviembre, de los medios públicos de comunicación audiovisual de Galicia. | 3 | as first published, then each change: 17 December 2011 to 7 April 2025; **repealed** 7 April 2025 by Ley 1/2025, de 14 de marzo (BOE-A-2025-6193) | 2025-12-19 |
| `decreto-legislativo-2015-002/` | Decreto Legislativo 2/2015, de 12 de febrero, por el que se aprueba el texto refundido de las disposiciones legales de la Comunidad Autónoma de Galicia en materia de igualdad. | 5 | oldest version available, then each change: 18 February 2016 to 31 December 2023; **repealed** 31 December 2023 by Ley 7/2023, de 30 de noviembre (BOE-A-2024-2663) | 2024-02-13 |

## Source

The consolidated legislation of the Agencia Estatal Boletín Oficial del Estado (BOE), through its open-data API, <https://www.boe.es/datosabiertos/api/legislacion-consolidada>. For each consolidated norm it gives every block of the text (article, disposition, annex, heading) with every version of that block, the day each version took effect (fecha_vigencia) and the norm that made it (id_norma). Each version here is the whole text as it stood on one of those days. The last column above is the BOE's own last-update date for the consolidated text.

## Dates

- Each commit is dated at **noon, Europe/Madrid, on the day the change took effect**: the fecha_vigencia the BOE gives the new block versions.
- A day on which the BOE records a new block version that changes no words is not a version here.
- Block versions with no in-force date (the BOE's 99999999, a date not yet fixed) are left out.
- An act's first commit is its first publication when the BOE's earliest text is the act as enacted; otherwise it is the oldest version the BOE holds.
- Versions that take effect after the retrieval day are on the `futuro` branch, never merged into `main`.

## Files

`<act>/art-005.md` is Artículo 5, `art-005-bis.md` Artículo 5 bis; `da-01.md` the Disposición adicional primera, `dt-` transitional, `dd-` repealing and `df-` final dispositions (`-unica` for "única"); `preambulo.md` the preamble, `firma.md` the signature, `anexo-*.md` the annexes. The book, title, chapter and section headings sit at the top of the file of the article that follows them. One paragraph per line; a table one line per row, cells separated by ` | `.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of the BOE's own text of that day, rebuilt from the source XML by a separate reader, and every file's text appears in it.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the norm that changed the text (a law, a decree-law, a ruling of the Constitutional Court), named by its title and BOE identifier, with an e-mail address that cannot exist (`<boe id>@boe.es.invalid`). The committer is always Lexifina.

## Limits

This is not an official publication. Only the texts published in the official journals are authentic. The history starts with the oldest text the BOE consolidates for each norm. Only the norms listed above are included; norms the BOE does not consolidate are not.
