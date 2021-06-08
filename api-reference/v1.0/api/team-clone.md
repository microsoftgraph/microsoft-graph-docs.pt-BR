---
title: Clonar uma equipe
description: Crie uma cópia de uma equipe. Essa operação também cria uma cópia do grupo correspondente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c4ef55620c8b13c001312ca391e553da60551a6a
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787440"
---
# <a name="clone-a-team"></a><span data-ttu-id="3b9d3-104">Clonar uma equipe</span><span class="sxs-lookup"><span data-stu-id="3b9d3-104">Clone a team</span></span>

<span data-ttu-id="3b9d3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b9d3-105">Namespace: microsoft.graph</span></span>



<span data-ttu-id="3b9d3-106">Crie uma cópia de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="3b9d3-106">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="3b9d3-107">Essa operação também cria uma cópia do grupo [correspondente](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="3b9d3-107">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="3b9d3-108">Você pode especificar quais partes da equipe clonar:</span><span class="sxs-lookup"><span data-stu-id="3b9d3-108">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="3b9d3-109">**apps** - Copia Microsoft Teams aplicativos instalados na equipe.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-109">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="3b9d3-110">**canais** – Copia a estrutura do canal (mas não as mensagens no canal).</span><span class="sxs-lookup"><span data-stu-id="3b9d3-110">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="3b9d3-111">**membros** – Copia os membros e proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-111">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="3b9d3-112">**configurações** – Copia todas as configurações dentro da equipe, juntamente com as principais configurações de grupo.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-112">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="3b9d3-113">**guias** – Copia as guias dentro dos canais.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-113">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="3b9d3-114">Quando as guias são clonadas, elas são colocadas em um estado não configurado - elas são exibidas na barra de guias no Microsoft Teams e, na primeira vez que você abri-las, você vai passar pela tela de configuração.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-114">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="3b9d3-115">(Se a pessoa que abre a guia não tiver permissão para configurar aplicativos, ela verá uma mensagem explicando que a guia não foi configurada.)</span><span class="sxs-lookup"><span data-stu-id="3b9d3-115">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="3b9d3-116">A clonagem é uma operação de longa duração.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-116">Cloning is a long-running operation.</span></span>
<span data-ttu-id="3b9d3-117">Depois que o clone POST retorna, você precisa OBTER a operação para ver se ela está "em execução" ou "bem-sucedida" ou "falhou". [](../resources/teamsasyncoperation.md)</span><span class="sxs-lookup"><span data-stu-id="3b9d3-117">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="3b9d3-118">Você deve continuar a OBTER até que o status não seja "em execução".</span><span class="sxs-lookup"><span data-stu-id="3b9d3-118">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="3b9d3-119">O atraso recomendado entre GETs é de 5 segundos.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-119">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b9d3-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b9d3-120">Permissions</span></span>

<span data-ttu-id="3b9d3-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b9d3-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b9d3-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b9d3-123">Permission type</span></span>      | <span data-ttu-id="3b9d3-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b9d3-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b9d3-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b9d3-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="3b9d3-126">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b9d3-126">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="3b9d3-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b9d3-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b9d3-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-128">Not supported.</span></span>    |
|<span data-ttu-id="3b9d3-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b9d3-129">Application</span></span>                            | <span data-ttu-id="3b9d3-130">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b9d3-130">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b9d3-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b9d3-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="3b9d3-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b9d3-132">Request headers</span></span>
| <span data-ttu-id="3b9d3-133">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b9d3-133">Header</span></span>       | <span data-ttu-id="3b9d3-134">Valor</span><span class="sxs-lookup"><span data-stu-id="3b9d3-134">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b9d3-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b9d3-135">Authorization</span></span>  | <span data-ttu-id="3b9d3-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3b9d3-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3b9d3-138">Content-Type</span></span>  | <span data-ttu-id="3b9d3-139">application/json</span><span class="sxs-lookup"><span data-stu-id="3b9d3-139">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b9d3-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b9d3-140">Request body</span></span>

| <span data-ttu-id="3b9d3-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b9d3-141">Property</span></span>     | <span data-ttu-id="3b9d3-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b9d3-142">Type</span></span>   |<span data-ttu-id="3b9d3-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b9d3-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b9d3-144">classificação</span><span class="sxs-lookup"><span data-stu-id="3b9d3-144">classification</span></span>|<span data-ttu-id="3b9d3-145">Cadeia de caracteres (opcional)</span><span class="sxs-lookup"><span data-stu-id="3b9d3-145">String (optional)</span></span>|<span data-ttu-id="3b9d3-146">Descreve uma classificação para o grupo (como baixo, médio ou alto impacto comercial).</span><span class="sxs-lookup"><span data-stu-id="3b9d3-146">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="3b9d3-147">Se a classificação não for especificada, a classificação será copiada da equipe/grupo original.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-147">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="3b9d3-148">description</span><span class="sxs-lookup"><span data-stu-id="3b9d3-148">description</span></span>|<span data-ttu-id="3b9d3-149">Cadeia de caracteres (opcional)</span><span class="sxs-lookup"><span data-stu-id="3b9d3-149">String (optional)</span></span>|<span data-ttu-id="3b9d3-150">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-150">An optional description for the group.</span></span> <span data-ttu-id="3b9d3-151">Se essa propriedade não for especificada, ela ficará em branco.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-151">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="3b9d3-152">displayName</span><span class="sxs-lookup"><span data-stu-id="3b9d3-152">displayName</span></span>|<span data-ttu-id="3b9d3-153">String</span><span class="sxs-lookup"><span data-stu-id="3b9d3-153">String</span></span>|<span data-ttu-id="3b9d3-p109">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-p109">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="3b9d3-157">mailNickname</span><span class="sxs-lookup"><span data-stu-id="3b9d3-157">mailNickname</span></span>|<span data-ttu-id="3b9d3-158">String</span><span class="sxs-lookup"><span data-stu-id="3b9d3-158">String</span></span>|<span data-ttu-id="3b9d3-159">O alias de email do grupo, exclusivo na organização.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-159">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="3b9d3-160">Essa propriedade deve ser especificada quando um grupo é criado.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-160">This property must be specified when a group is created.</span></span> <span data-ttu-id="3b9d3-161">Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-161">Supports $filter.</span></span> <span data-ttu-id="3b9d3-162">Se essa propriedade não for especificada, ela será calculada a partir do displayName.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-162">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="3b9d3-163">Problema conhecido: essa propriedade é ignorada no momento.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-163">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="3b9d3-164">partsToClone</span><span class="sxs-lookup"><span data-stu-id="3b9d3-164">partsToClone</span></span>| [<span data-ttu-id="3b9d3-165">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="3b9d3-165">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="3b9d3-166">Uma lista separada por vírgulas das partes a ser clonada.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-166">A comma-separated list of the parts to clone.</span></span> <span data-ttu-id="3b9d3-167">As partes legais são "aplicativos, guias, configurações, canais, membros".</span><span class="sxs-lookup"><span data-stu-id="3b9d3-167">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="3b9d3-168">visibility</span><span class="sxs-lookup"><span data-stu-id="3b9d3-168">visibility</span></span>|<span data-ttu-id="3b9d3-169">[teamVisibilityType](../resources/teamvisibilitytype.md) (opcional)</span><span class="sxs-lookup"><span data-stu-id="3b9d3-169">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="3b9d3-170">Especifica a visibilidade do grupo.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-170">Specifies the visibility of the group.</span></span> <span data-ttu-id="3b9d3-171">Os valores possíveis são: **Private**, **Public**.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-171">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="3b9d3-172">Se a visibilidade não for especificada, a visibilidade será copiada da equipe/grupo original.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-172">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="3b9d3-173">Se a equipe que está sendo clonada for uma equipe **educationClass,** o parâmetro de visibilidade será ignorado e a visibilidade do novo grupo será definida como HiddenMembership.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-173">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="3b9d3-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b9d3-174">Response</span></span>

<span data-ttu-id="3b9d3-175">Se tiver êxito, este método retornará um código `202 Accepted` de resposta com um header Location: apontando para o recurso [de](../resources/teamsasyncoperation.md) operação.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-175">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="3b9d3-176">Quando a operação for concluída, o recurso de operação dirá a id da equipe criada.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-176">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="3b9d3-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b9d3-177">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3b9d3-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b9d3-178">Request</span></span>
<span data-ttu-id="3b9d3-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3b9d3-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b9d3-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "clone_team"
}-->
```http
POST /teams/{id}/clone
Content-Type: application/json

{  
     "displayName": "Library Assist",
     "description": "Self help community for library",
     "mailNickname": "libassist",
     "partsToClone": "apps,tabs,settings,channels,members",
     "visibility": "public"
}
```
# <a name="c"></a>[<span data-ttu-id="3b9d3-181">C#</span><span class="sxs-lookup"><span data-stu-id="3b9d3-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/clone-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b9d3-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b9d3-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/clone-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b9d3-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b9d3-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/clone-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b9d3-184">Java</span><span class="sxs-lookup"><span data-stu-id="3b9d3-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/clone-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b9d3-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b9d3-185">Response</span></span>
<span data-ttu-id="3b9d3-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-186">The following is an example of the response.</span></span> <span data-ttu-id="3b9d3-187">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-187">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

