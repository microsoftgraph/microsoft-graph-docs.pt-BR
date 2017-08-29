# <a name="get-a-site-resource"></a><span data-ttu-id="4ba0d-101">Obter um recurso de site</span><span class="sxs-lookup"><span data-stu-id="4ba0d-101">Get a site resource</span></span>

<span data-ttu-id="4ba0d-p101">Recupere as propriedades e as relações de um recurso [site][]. Um recurso **site** representa um site de equipe no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4ba0d-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

<span data-ttu-id="4ba0d-104">[site]: ../resources/site.md</span><span class="sxs-lookup"><span data-stu-id="4ba0d-104">[site]: ../resources/site.md</span></span>

<span data-ttu-id="4ba0d-105">Um **site** é endereçado para ser um identificador exclusivo que é uma ID composta dos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="4ba0d-105">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="4ba0d-106">Hostname do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="4ba0d-106">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="4ba0d-107">ID exclusiva do conjunto de sites (guid)</span><span class="sxs-lookup"><span data-stu-id="4ba0d-107">Site collection unique ID (guid)</span></span>
* <span data-ttu-id="4ba0d-108">ID exclusiva do site (guid)</span><span class="sxs-lookup"><span data-stu-id="4ba0d-108">Site unique ID (guid)</span></span>

<span data-ttu-id="4ba0d-109">Há também um identificador de site reservado, `root`, que sempre faz referência ao site raiz de um determinado destino da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="4ba0d-109">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="4ba0d-110">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="4ba0d-110">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="4ba0d-111">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="4ba0d-111">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ba0d-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ba0d-112">Permissions</span></span>

<span data-ttu-id="4ba0d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4ba0d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4ba0d-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ba0d-115">Permission type</span></span>      | <span data-ttu-id="4ba0d-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ba0d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ba0d-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ba0d-117">Delegated (work or school account)</span></span> | <span data-ttu-id="4ba0d-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ba0d-118">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4ba0d-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ba0d-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ba0d-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ba0d-120">Not supported.</span></span>    |
|<span data-ttu-id="4ba0d-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ba0d-121">Application</span></span> | <span data-ttu-id="4ba0d-122">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ba0d-122">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="4ba0d-123">Obter o site raiz do locatário</span><span class="sxs-lookup"><span data-stu-id="4ba0d-123">Get the tenant's root site</span></span>

<span data-ttu-id="4ba0d-124">Para acessar o site raiz do SharePoint dentro de um locatário:</span><span class="sxs-lookup"><span data-stu-id="4ba0d-124">To access the root SharePoint site within a tenant:</span></span>

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="4ba0d-125">Acesse um site pela URL relativa do servidor</span><span class="sxs-lookup"><span data-stu-id="4ba0d-125">Access a site by server-relative URL</span></span>

<span data-ttu-id="4ba0d-126">Se você tiver a URL relativa do servidor para um recurso **site**, crie uma solicitação da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="4ba0d-126">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="4ba0d-127">Acesse um site de equipe do grupo</span><span class="sxs-lookup"><span data-stu-id="4ba0d-127">Access a group team site</span></span>

<span data-ttu-id="4ba0d-128">Para acessar o site de equipe de um [grupo](../resources/group.md):</span><span class="sxs-lookup"><span data-stu-id="4ba0d-128">To access the team site for a [group](../resources/group.md):</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="4ba0d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ba0d-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4ba0d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ba0d-130">Request</span></span>

<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}
```

##### <a name="response"></a><span data-ttu-id="4ba0d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ba0d-131">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "d297964f-d325-424b-a002-f54048a4622e",
    "name": "OneDrive / SharePoint Team",
    "description": "Collaboration site for the OneDrive and SharePoint team",
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/Get site by ID"
} -->
