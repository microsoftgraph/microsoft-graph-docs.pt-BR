
<!-- markdownlint-disable MD041-->

Quando um aplicativo consulta um relacionamento que retorna uma coleção de tipos de directoryobject, se ele não tiver permissão para ler um determinado tipo derivado (como dispositivo), os membros desse tipo serão retornados, mas com informações limitadas. Com esse comportamento, os aplicativos podem solicitar as permissões menos privilegiadas necessárias, em vez de confiar no conjunto de permissões de Directory. *. Para obter detalhes, consulte [informações limitadas retornadas para objetos membro inacessíveis](/graph/permissions-reference#limited-information-returned-for-inaccessible-member-objects).

