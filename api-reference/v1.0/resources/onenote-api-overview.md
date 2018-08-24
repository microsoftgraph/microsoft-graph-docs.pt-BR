# <a name="use-the-onenote-rest-api"></a>Usar a API REST do OneNote

O Microsoft Graph permite que o seu aplicativo obtenha acesso autorizado aos blocos de anotações, seções e páginas de um usuário do OneNote em uma conta pessoal ou da organização. Com as [permissões delegadas ou de aplicativos apropriadas](../../../concepts/permissions_reference.md#notes-permissions), seu aplicativo pode acessar os dados de OneNote do usuário conectado ou de qualquer usuário em um locatário.

## <a name="root-url"></a>URL raiz
A URL raiz do serviço do OneNote usa o formato a seguir para todas as chamadas para a API do OneNote.
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
O segmento `version` na URL representa a versão do Microsoft Graph que você deseja usar:

- `v1.0` serve para o código de produção estável.
- `beta` serve para experimentar um recurso que está em desenvolvimento. Recursos e funcionalidades no ponto de extremidade beta podem ser alterados; não recomendamos que você use-o em seu código de produção.

A localização pode ser os blocos de anotações do usuário no Office 365 ou no OneDrive do consumidor, blocos de anotações de grupo ou blocos de anotações de equipe hospedados no site do SharePoint no Office 365. 

![Pilha de desenvolvimento da API do OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>Blocos de anotações do usuário
Para acessar os blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- `me` serve para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado).
- `users/{id}` serve para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual. Use a API [usuários](users.md).
> **Observação:** para obter as ids de usuário, faça uma solicitação GET em `https://graph.microsoft.com/v1.0/users`.

### <a name="group-notebooks"></a>Blocos de anotações de grupo
Para acessar os blocos de anotações que pertencem a um grupo, use a seguinte URL raiz de serviço:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>Blocos de anotações do site do SharePoint

Para acessar os blocos de anotações que pertencem a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

