# <a name="group-getmembergroups"></a><span data-ttu-id="a519e-101">grupo: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="a519e-101">group: getMemberGroups</span></span>

<span data-ttu-id="a519e-p101">Retorne todos os grupos dos quais o grupo especificado é membro. A verificação é transitiva, diferentemente da leitura da propriedade de navegação [memberOf](../api/group_list_memberof.md), que retorna somente os grupos dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="a519e-p101">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group_list_memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="a519e-p102">Esta função dá suporte ao Office 365 e a outros tipos de grupos provisionados no Azure AD. O número máximo de grupos de que cada solicitação pode retornar é 2046. Observe que os Grupos do Office 365 não podem conter grupos, portanto associações em um Grupo do Office 365 sempre são diretas.</span><span class="sxs-lookup"><span data-stu-id="a519e-p102">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="a519e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a519e-108">Permissions</span></span>

<span data-ttu-id="a519e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a519e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="a519e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a519e-111">Permission type</span></span>                        | <span data-ttu-id="a519e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a519e-112">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="a519e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a519e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a519e-114">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a519e-114">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="a519e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a519e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a519e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a519e-116">Not supported.</span></span>                                                                              |
| <span data-ttu-id="a519e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a519e-117">Application</span></span>                            | <span data-ttu-id="a519e-118">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a519e-118">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="a519e-119">**Observação:** Essa API atualmente requer a permissão `Directory.Read.All` ou superior.</span><span class="sxs-lookup"><span data-stu-id="a519e-119">Note: This API currently requires the Directory.Read.All permission or higher.</span></span> <span data-ttu-id="a519e-120">Usando a permissão `Group.Read.All` retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="a519e-120">Using the Group.Read.All permission will return an error.</span></span> <span data-ttu-id="a519e-121">Este é um bug conhecido.</span><span class="sxs-lookup"><span data-stu-id="a519e-121">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="a519e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a519e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="a519e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a519e-123">Request headers</span></span>

| <span data-ttu-id="a519e-124">Nome</span><span class="sxs-lookup"><span data-stu-id="a519e-124">Name</span></span>          | <span data-ttu-id="a519e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="a519e-125">Type</span></span>   | <span data-ttu-id="a519e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="a519e-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="a519e-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="a519e-127">Authorization</span></span> | <span data-ttu-id="a519e-128">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="a519e-128">string</span></span> | <span data-ttu-id="a519e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a519e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a519e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a519e-131">Request body</span></span>

<span data-ttu-id="a519e-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a519e-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a519e-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a519e-133">Parameter</span></span>           | <span data-ttu-id="a519e-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="a519e-134">Type</span></span>    | <span data-ttu-id="a519e-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="a519e-135">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="a519e-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a519e-136">securityEnabledOnly</span></span> | <span data-ttu-id="a519e-137">Booleano</span><span class="sxs-lookup"><span data-stu-id="a519e-137">Boolean</span></span> | <span data-ttu-id="a519e-p106">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="a519e-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="a519e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a519e-140">Response</span></span>

<span data-ttu-id="a519e-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="a519e-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="a519e-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a519e-142">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a519e-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a519e-143">Request</span></span>

<span data-ttu-id="a519e-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a519e-144">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="a519e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a519e-145">Response</span></span>

<span data-ttu-id="a519e-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a519e-146">The following is an example of the response.</span></span>

> <span data-ttu-id="a519e-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a519e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
