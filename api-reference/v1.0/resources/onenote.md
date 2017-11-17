# <a name="onenote-resource-type"></a><span data-ttu-id="2f445-101">tipo de recurso do onenote</span><span class="sxs-lookup"><span data-stu-id="2f445-101">onenote resource type</span></span>

<span data-ttu-id="2f445-102">O ponto de entrada para os recursos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="2f445-102">The entry point for OneNote resources.</span></span>

<span data-ttu-id="2f445-103">Todas as chamadas para o serviço do OneNote pela API do Microsoft Graph usam essa URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="2f445-103">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="2f445-104">A localização pode ser blocos de anotações do usuário no Office 365 ou OneDrive do consumidor, blocos de anotações de grupo ou blocos de anotações hospedado no site de equipe do SharePoint no Office 365.</span><span class="sxs-lookup"><span data-stu-id="2f445-104">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="2f445-105">**Blocos de anotações do usuário** Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:</span><span class="sxs-lookup"><span data-stu-id="2f445-105">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="2f445-106">**Blocos de anotações de grupo** para acessar blocos de anotações que pertencem a um grupo, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="2f445-106">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="2f445-107">**Blocos de anotações do site do SharePoint** para acessar blocos de anotações que pertencem a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="2f445-107">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="2f445-108">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f445-108">Authorization</span></span>

<span data-ttu-id="2f445-109">Para obter informações sobre as permissões necessárias para trabalhar com o APIs do OneNote, confira [Permissões de anotações](../../../concepts/permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="2f445-109">For information about the permissions required to work with OneNote APIs, see [Notes permissions](../../../concepts/permissions_reference.md#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="2f445-110">Relações</span><span class="sxs-lookup"><span data-stu-id="2f445-110">Relationships</span></span>
| <span data-ttu-id="2f445-111">Relação</span><span class="sxs-lookup"><span data-stu-id="2f445-111">Relationship</span></span> | <span data-ttu-id="2f445-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f445-112">Type</span></span>   |<span data-ttu-id="2f445-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f445-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f445-114">notebooks</span><span class="sxs-lookup"><span data-stu-id="2f445-114">notebooks</span></span>|<span data-ttu-id="2f445-115">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="2f445-115">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="2f445-p101">A coleção de blocos de anotações do OneNote que pertencem ao usuário ou ao grupo. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f445-p101">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="2f445-119">operations</span><span class="sxs-lookup"><span data-stu-id="2f445-119">operations</span></span>|<span data-ttu-id="2f445-120">Coleção [Operation](onenoteoperation.md)</span><span class="sxs-lookup"><span data-stu-id="2f445-120">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="2f445-p102">O status das operações do OneNote. Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status das operações longas se o cabeçalho `Operation-Location` for retornado na resposta. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f445-p102">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="2f445-125">páginas</span><span class="sxs-lookup"><span data-stu-id="2f445-125">pages</span></span>|<span data-ttu-id="2f445-126">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="2f445-126">[Page](page.md) collection</span></span>|<span data-ttu-id="2f445-p103">As páginas em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f445-p103">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="2f445-130">recursos</span><span class="sxs-lookup"><span data-stu-id="2f445-130">resources</span></span>|<span data-ttu-id="2f445-131">Coleção [Resource](resource.md)</span><span class="sxs-lookup"><span data-stu-id="2f445-131">[Resource](resource.md) collection</span></span> |<span data-ttu-id="2f445-p104">A imagem e outros recursos de arquivos nas páginas do OneNote. Não há suporte para a obtenção de uma coleção de recursos, mas você pode [obter o conteúdo de um recurso binário específico](resource.md). Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f445-p104">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="2f445-136">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="2f445-136">sectionGroups</span></span>|<span data-ttu-id="2f445-137">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="2f445-137">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="2f445-p105">Os grupos de seção em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f445-p105">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="2f445-141">seções</span><span class="sxs-lookup"><span data-stu-id="2f445-141">sections</span></span>|<span data-ttu-id="2f445-142">Coleção [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="2f445-142">[Section](section.md) collection</span></span>|<span data-ttu-id="2f445-p106">As seções em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f445-p106">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="2f445-146">Métodos</span><span class="sxs-lookup"><span data-stu-id="2f445-146">Methods</span></span>

| <span data-ttu-id="2f445-147">Método</span><span class="sxs-lookup"><span data-stu-id="2f445-147">Method</span></span>           | <span data-ttu-id="2f445-148">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2f445-148">Return Type</span></span>    |<span data-ttu-id="2f445-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f445-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f445-150">Create notebook</span><span class="sxs-lookup"><span data-stu-id="2f445-150">Create notebook</span></span>](../api/onenote_post_notebooks.md) |[<span data-ttu-id="2f445-151">Notebook</span><span class="sxs-lookup"><span data-stu-id="2f445-151">Notebook</span></span>](notebook.md)| <span data-ttu-id="2f445-152">Crie um bloco de anotações postando na coleção notebooks.</span><span class="sxs-lookup"><span data-stu-id="2f445-152">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="2f445-153">List notebooks</span><span class="sxs-lookup"><span data-stu-id="2f445-153">List notebooks</span></span>](../api/onenote_list_notebooks.md) |<span data-ttu-id="2f445-154">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="2f445-154">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="2f445-155">Obter uma coleção de blocos de anotações.</span><span class="sxs-lookup"><span data-stu-id="2f445-155">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="2f445-156">Create page</span><span class="sxs-lookup"><span data-stu-id="2f445-156">Create page</span></span>](../api/onenote_post_pages.md) |[<span data-ttu-id="2f445-157">Page</span><span class="sxs-lookup"><span data-stu-id="2f445-157">Page</span></span>](page.md)| <span data-ttu-id="2f445-158">Crie uma página postando na coleção pages.</span><span class="sxs-lookup"><span data-stu-id="2f445-158">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="2f445-159">List pages</span><span class="sxs-lookup"><span data-stu-id="2f445-159">List pages</span></span>](../api/onenote_list_pages.md) |<span data-ttu-id="2f445-160">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="2f445-160">[Page](page.md) collection</span></span>| <span data-ttu-id="2f445-161">Obter uma coleção de páginas.</span><span class="sxs-lookup"><span data-stu-id="2f445-161">Get a collection of pages.</span></span>|
|[<span data-ttu-id="2f445-162">List section groups</span><span class="sxs-lookup"><span data-stu-id="2f445-162">List section groups</span></span>](../api/onenote_list_sectiongroups.md) |<span data-ttu-id="2f445-163">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="2f445-163">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="2f445-164">Obter uma coleção de grupos de seção.</span><span class="sxs-lookup"><span data-stu-id="2f445-164">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="2f445-165">List sections</span><span class="sxs-lookup"><span data-stu-id="2f445-165">List sections</span></span>](../api/onenote_list_sections.md) |<span data-ttu-id="2f445-166">Coleção [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="2f445-166">[Section](section.md) collection</span></span>| <span data-ttu-id="2f445-167">Obter uma coleção de seções.</span><span class="sxs-lookup"><span data-stu-id="2f445-167">Get a collection of sections.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
