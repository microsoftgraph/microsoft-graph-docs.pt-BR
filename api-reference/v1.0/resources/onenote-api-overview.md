# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="37a9e-101">Usar a API REST do OneNote</span><span class="sxs-lookup"><span data-stu-id="37a9e-101">Use the OneNote REST API</span></span>

<span data-ttu-id="37a9e-102">O Microsoft Graph permite que o seu aplicativo obtenha acesso autorizado aos blocos de anotações, seções e páginas de um usuário do OneNote em uma conta pessoal ou da organização.</span><span class="sxs-lookup"><span data-stu-id="37a9e-102">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="37a9e-103">Com as [permissões delegadas ou de aplicativos apropriadas](../../../concepts/permissions_reference.md#notes-permissions), seu aplicativo pode acessar os dados de OneNote do usuário conectado ou de qualquer usuário em um locatário.</span><span class="sxs-lookup"><span data-stu-id="37a9e-103">With the [appropriate delegated or application permissions](../../../concepts/permissions_reference.md#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span>

## <a name="root-url"></a><span data-ttu-id="37a9e-104">URL raiz</span><span class="sxs-lookup"><span data-stu-id="37a9e-104">Root URL</span></span>
<span data-ttu-id="37a9e-105">A URL raiz do serviço do OneNote usa o formato a seguir para todas as chamadas para a API do OneNote.</span><span class="sxs-lookup"><span data-stu-id="37a9e-105">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
<span data-ttu-id="37a9e-106">O segmento `version` na URL representa a versão do Microsoft Graph que você deseja usar:</span><span class="sxs-lookup"><span data-stu-id="37a9e-106">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span>

- <span data-ttu-id="37a9e-107">`v1.0` serve para o código de produção estável.</span><span class="sxs-lookup"><span data-stu-id="37a9e-107">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="37a9e-108">`beta` serve para experimentar um recurso que está em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="37a9e-108">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="37a9e-109">Recursos e funcionalidades no ponto de extremidade beta podem ser alterados; não recomendamos que você use-o em seu código de produção.</span><span class="sxs-lookup"><span data-stu-id="37a9e-109">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="37a9e-110">A localização pode ser os blocos de anotações do usuário no Office 365 ou no OneDrive do consumidor, blocos de anotações de grupo ou blocos de anotações de equipe hospedados no site do SharePoint no Office 365.</span><span class="sxs-lookup"><span data-stu-id="37a9e-110">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![Pilha de desenvolvimento da API do OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="37a9e-112">Blocos de anotações do usuário</span><span class="sxs-lookup"><span data-stu-id="37a9e-112">User notebooks</span></span>
<span data-ttu-id="37a9e-113">Para acessar os blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:</span><span class="sxs-lookup"><span data-stu-id="37a9e-113">User notebooks To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="37a9e-114">`me` serve para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado).</span><span class="sxs-lookup"><span data-stu-id="37a9e-114">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="37a9e-115">`users/{id}` serve para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="37a9e-115">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="37a9e-116">Use a API [usuários](users.md).</span><span class="sxs-lookup"><span data-stu-id="37a9e-116">[Use the Planner API](users.md)</span></span>
> <span data-ttu-id="37a9e-117">**Observação:** para obter as ids de usuário, faça uma solicitação GET em `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="37a9e-117">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="37a9e-118">Blocos de anotações de grupo</span><span class="sxs-lookup"><span data-stu-id="37a9e-118">Group notebooks</span></span>
<span data-ttu-id="37a9e-119">Para acessar os blocos de anotações que pertencem a um grupo, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="37a9e-119">Group notebooks To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="37a9e-120">Blocos de anotações do site do SharePoint</span><span class="sxs-lookup"><span data-stu-id="37a9e-120">SharePoint site notebooks</span></span>

<span data-ttu-id="37a9e-121">Para acessar os blocos de anotações que pertencem a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="37a9e-121">SharePoint site notebooks To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

