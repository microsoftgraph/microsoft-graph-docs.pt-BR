# <a name="list-apps-in-team"></a><span data-ttu-id="c4a3d-101">Lista de aplicativos na equipe</span><span class="sxs-lookup"><span data-stu-id="c4a3d-101">List apps in team</span></span>



<span data-ttu-id="c4a3d-102">Recupere a lista de [aplicativos instalados](../resources/teamsappinstallation.md) na [equipe](../resources/team.md)de especificado.</span><span class="sxs-lookup"><span data-stu-id="c4a3d-102">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4a3d-103">Permissions</span><span class="sxs-lookup"><span data-stu-id="c4a3d-103">Permissions</span></span>

<span data-ttu-id="c4a3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c4a3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c4a3d-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4a3d-106">Permission type</span></span>      | <span data-ttu-id="c4a3d-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4a3d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4a3d-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4a3d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c4a3d-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4a3d-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c4a3d-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4a3d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4a3d-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4a3d-111">Not supported.</span></span>    |
|<span data-ttu-id="c4a3d-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4a3d-112">Application</span></span> | <span data-ttu-id="c4a3d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4a3d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4a3d-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4a3d-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4a3d-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c4a3d-115">Optional query parameters</span></span>

<span data-ttu-id="c4a3d-116">Este método oferece suporte a $filter, $select, e $expand [OData parâmetros de consulta](../../../concepts/query_parameters.md) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c4a3d-116">This method supports the $filter, $select, and $expand [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4a3d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a3d-117">Request headers</span></span>

| <span data-ttu-id="c4a3d-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4a3d-118">Header</span></span>       | <span data-ttu-id="c4a3d-119">Valor</span><span class="sxs-lookup"><span data-stu-id="c4a3d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c4a3d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4a3d-120">Authorization</span></span>  | <span data-ttu-id="c4a3d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4a3d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c4a3d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a3d-123">Request body</span></span>

<span data-ttu-id="c4a3d-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4a3d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4a3d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4a3d-125">Response</span></span>

<span data-ttu-id="c4a3d-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [teamsApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4a3d-126">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4a3d-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4a3d-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4a3d-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a3d-128">Request</span></span>

<span data-ttu-id="c4a3d-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4a3d-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="c4a3d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4a3d-130">Response</span></span>

<span data-ttu-id="c4a3d-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c4a3d-131">The following is an example of the response.</span></span>
><span data-ttu-id="c4a3d-132">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c4a3d-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c4a3d-133">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4a3d-133">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="c4a3d-134">Example - obtendo os nomes dos aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="c4a3d-134">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="c4a3d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a3d-135">Request</span></span>

<span data-ttu-id="c4a3d-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4a3d-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="c4a3d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4a3d-137">Response</span></span>

<span data-ttu-id="c4a3d-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c4a3d-138">The following is an example of the response.</span></span>

><span data-ttu-id="c4a3d-139">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c4a3d-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c4a3d-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4a3d-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
    "value": [
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "displayName": "OneNote",
                "version": "1.0.0"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZmQ5MjVhMC0zNTdmLTRkMjUtODQ1Ni1iMzAyMmFhYTQxYTk=",
            "teamsAppDefinition": {
                "id": "MGZkOTI1YTAtMzU3Zi00ZDI1LTg0NTYtYjMwMjJhYWE0MWE5IyMxLjc=",
                "teamsAppId": "0fd925a0-357f-4d25-8456-b3022aaa41a9",
                "displayName": "SurveyMonkey",
                "version": "1.7"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMyYTUyNzcwMy0xZjZmLTQ1NTktYTMzMi1kOGE3ZDI4OGNkODg=",
            "teamsAppDefinition": {
                "id": "MmE1Mjc3MDMtMWY2Zi00NTU5LWEzMzItZDhhN2QyODhjZDg4IyMxLjA=",
                "teamsAppId": "2a527703-1f6f-4559-a332-d8a7d288cd88",
                "displayName": "SharePoint",
                "version": "1.0"
            }
        }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->