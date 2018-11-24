# <a name="add-app-to-team"></a><span data-ttu-id="d0db2-101">Adicionar o aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="d0db2-101">Add app to team</span></span>



<span data-ttu-id="d0db2-102">Instala um [aplicativo](../resources/teamsapp.md) para a [equipe](../resources/team.md)de especificado.</span><span class="sxs-lookup"><span data-stu-id="d0db2-102">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d0db2-103">Permissions</span><span class="sxs-lookup"><span data-stu-id="d0db2-103">Permissions</span></span>
<span data-ttu-id="d0db2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d0db2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d0db2-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0db2-106">Permission type</span></span>      | <span data-ttu-id="d0db2-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0db2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0db2-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0db2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d0db2-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0db2-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0db2-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0db2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0db2-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0db2-111">Not supported.</span></span>    |
|<span data-ttu-id="d0db2-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0db2-112">Application</span></span> | <span data-ttu-id="d0db2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0db2-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0db2-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0db2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="d0db2-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0db2-115">Request headers</span></span>
| <span data-ttu-id="d0db2-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0db2-116">Header</span></span>       | <span data-ttu-id="d0db2-117">Valor</span><span class="sxs-lookup"><span data-stu-id="d0db2-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d0db2-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0db2-118">Authorization</span></span>  | <span data-ttu-id="d0db2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0db2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0db2-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0db2-121">Request body</span></span>

| <span data-ttu-id="d0db2-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0db2-122">Property</span></span>     | <span data-ttu-id="d0db2-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0db2-123">Type</span></span>   |<span data-ttu-id="d0db2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0db2-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0db2-125">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d0db2-125">teamsApp</span></span>| [<span data-ttu-id="d0db2-126">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d0db2-126">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="d0db2-127">Para adicionar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d0db2-127">The app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="d0db2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0db2-128">Response</span></span>

<span data-ttu-id="d0db2-129">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="d0db2-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d0db2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0db2-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d0db2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0db2-131">Request</span></span>
<span data-ttu-id="d0db2-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0db2-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="d0db2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0db2-133">Response</span></span>
<span data-ttu-id="d0db2-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d0db2-134">The following is an example of the response.</span></span> <span data-ttu-id="d0db2-135">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="d0db2-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d0db2-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0db2-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="d0db2-137">Veja também</span><span class="sxs-lookup"><span data-stu-id="d0db2-137">See also</span></span>

