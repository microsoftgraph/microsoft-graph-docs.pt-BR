# <a name="working-with-education-apis-in-microsoft-graph"></a>Como trabalhar com APIs de educação no Microsoft Graph

As APIs de educação no Microsoft Graph aprimoram os recursos e dados do Office 365 com informações que são relevantes para cenários de educação, incluindo escolas, alunos, professores, aulas e matrículas. Isso facilita a criação de soluções que se integram aos recursos educacionais.

As APIs de educação incluem recursos de escalação e recursos de atribuições que podem ser usados para interação com os serviços de escalação no Microsoft Teams. Você pode usar esses recursos para gerenciar a lista de participantes de uma escola.

## <a name="authorization"></a>Autorização

Para chamar as APIs de educação no Microsoft Graph, o aplicativo precisará adquirir um token de acesso. Para obter detalhes sobre tokens de acesso, confira [Obter tokens de acesso para chamar o Microsoft Graph](https://developer.microsoft.com/pt-BR/graph/docs/concepts/auth_overview). O aplicativo também precisará das permissões apropriadas. Para saber mais, confira [Permissões de educação](../../../concepts/permissions_reference.md#education-permissions). 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a>Permissões de aplicativo para permitir o consentimento dos administradores de TI da escola 

Para implantar os aplicativos que são integrados às APIs de educação do Microsoft Graph, primeiramente, os administradores de TI da escola devem dar consentimento para as permissões solicitadas pelo aplicativo. Esse consentimento deve ser concedido apenas uma vez, a menos que as permissões mudem. Após o consentimento do administrador, o aplicativo está provisionado para todos os usuários no locatário.

Para acionar uma caixa de diálogo de consentimento, use a chamada REST a seguir.

```
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

|Parâmetro|Descrição|
|:--------|:----------|
|Tenant|ID do locatário da escola. Use a ID completa, que inclui onmicrosoft.com.|
|clientId|ID do cliente do aplicativo.|
|redirectUrl|URL de redirecionamento do aplicativo.|


## <a name="rostering"></a>Lista de participantes

As APIs de lista de participantes permitem extrair dados do locatário do Office 365 de uma escola provisionado com o [Microsoft School Data Sync](https://sds.microsoft.com/). Essas APIs fornecem acesso às informações sobre escolas, seções, professores, alunos e listas de participantes. As APIs dão suporte a cenários somente aplicativo (sincronismo) e a cenários de aplicativo mais usuário (interativo). As APIs que dão suporte a cenários interativos aplicam políticas RBAC apropriadas da região, com base na função do usuário que está chamando a API. Isso fornece uma API consistente e uma superfície mínima de política, independentemente da configuração administrativa nos locatários. Além disso, as APIs também fornecem permissões específicas de educação, de modo a garantir que o usuário certo tenha acesso aos dados.

Você pode usar as APIs de escalação para permitir que um usuário do aplicativo saiba:

- Quem eu sou
- Quais aulas eu frequento ou ministro
- O que preciso fazer e quando

As APIs de escalação fornecem os seguintes recursos-chave:

- [educationSchool](educationschool.md) – representa a escola.
- [educationClass](educationclass.md) – representa uma aula em uma escola.
- [educationTerm](educationterm.md) – representa uma parte designada do ano acadêmico.
- [educationTeacher](educationteacher.md) – representa um usuário com a função principal de ‘Professor’.
- [educationStudent](educationstudent.md) – representa um usuário com a função principal de 'aluno'.

As APIs de escalação dão suporte aos seguintes cenários:

- [Listar todas as escolas](../api/educationroot_list_schools.md) 
- [Listar escolas nas quais uma aula é ministrada](../api/educationclass_list_schools.md)
- [Listar escolas para um usuário](../api/educationuser_list_schools.md)
- [Obter todas as aulas](../api/educationroot_list_classes.md )
- [Obter aulas em um escola](../api/educationschool_list_classes.md)
- [Listar aulas para um usuário](../api/educationuser_list_classes.md)
- [Adicionar aulas a uma escola](../api/educationschool_post_classes.md)
- [Obter alunos e professores para uma aula](../api/educationclass_list_members.md)
- [Adicionar membros a uma aula](../api/educationclass_post_members.md) 
- [Listar professores para uma aula](../api/educationclass_list_teachers.md)
- [Obter usuários em uma escola](../api/educationschool_list_users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="next-steps"></a>Próximas etapas
Use as APIs de educação do Microsoft Graph para criar soluções de educação que acessam listas de participantes da escola. Para saber mais:

- Explore os recursos e os métodos mais úteis para seu cenário.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/pt-BR/graph/graph-explorer).

