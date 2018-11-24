# <a name="delete-app-from-team"></a><span data-ttu-id="eece0-101">Excluir o aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="eece0-101">Delete app from team</span></span>



<span data-ttu-id="eece0-102">Desinstala um [aplicativo](../resources/teamsappinstallation.md) da [equipe](../resources/team.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="eece0-102">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eece0-103">Permissions</span><span class="sxs-lookup"><span data-stu-id="eece0-103">Permissions</span></span>
<span data-ttu-id="eece0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eece0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eece0-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eece0-106">Permission type</span></span>      | <span data-ttu-id="eece0-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eece0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eece0-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eece0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="eece0-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eece0-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="eece0-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eece0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eece0-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eece0-111">Not supported.</span></span>    |
|<span data-ttu-id="eece0-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eece0-112">Application</span></span> | <span data-ttu-id="eece0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eece0-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eece0-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eece0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="eece0-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eece0-115">Request headers</span></span>
| <span data-ttu-id="eece0-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eece0-116">Header</span></span>       | <span data-ttu-id="eece0-117">Valor</span><span class="sxs-lookup"><span data-stu-id="eece0-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eece0-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="eece0-118">Authorization</span></span>  | <span data-ttu-id="eece0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eece0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eece0-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eece0-121">Request body</span></span>
<span data-ttu-id="eece0-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eece0-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eece0-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="eece0-123">Response</span></span>

<span data-ttu-id="eece0-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eece0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eece0-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eece0-126">Example</span></span>
#### <a name="request"></a><span data-ttu-id="eece0-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eece0-127">Request</span></span>
<span data-ttu-id="eece0-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eece0-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="eece0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="eece0-129">Response</span></span>
<span data-ttu-id="eece0-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eece0-130">The following is an example of the response.</span></span> <span data-ttu-id="eece0-131">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="eece0-131">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="eece0-132">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eece0-132">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
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
