---
title: Clonar uma equipe
description: Crie uma cópia de uma equipe. Essa operação também cria uma cópia do grupo correspondente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6299d1e7ecf828ee6587c4a69796021f1905dfd5
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786857"
---
# <a name="clone-a-team"></a><span data-ttu-id="746fb-104">Clonar uma equipe</span><span class="sxs-lookup"><span data-stu-id="746fb-104">Clone a team</span></span>

<span data-ttu-id="746fb-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="746fb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="746fb-106">Crie uma cópia de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="746fb-106">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="746fb-107">Essa operação também cria uma cópia do grupo [correspondente](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="746fb-107">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="746fb-108">Você pode especificar quais partes da equipe clonar:</span><span class="sxs-lookup"><span data-stu-id="746fb-108">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="746fb-109">**apps** - Copia Microsoft Teams aplicativos instalados na equipe.</span><span class="sxs-lookup"><span data-stu-id="746fb-109">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="746fb-110">**canais** – Copia a estrutura do canal (mas não as mensagens no canal).</span><span class="sxs-lookup"><span data-stu-id="746fb-110">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="746fb-111">**membros** – Copia os membros e proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="746fb-111">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="746fb-112">**configurações** – Copia todas as configurações dentro da equipe, juntamente com as principais configurações de grupo.</span><span class="sxs-lookup"><span data-stu-id="746fb-112">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="746fb-113">**guias** – Copia as guias dentro dos canais.</span><span class="sxs-lookup"><span data-stu-id="746fb-113">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="746fb-114">Quando as guias são clonadas, elas são colocadas em um estado não configurado - elas são exibidas na barra de guias no Microsoft Teams e, na primeira vez que você abri-las, você vai passar pela tela de configuração.</span><span class="sxs-lookup"><span data-stu-id="746fb-114">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="746fb-115">(Se a pessoa que abre a guia não tiver permissão para configurar aplicativos, ela verá uma mensagem explicando que a guia não foi configurada.)</span><span class="sxs-lookup"><span data-stu-id="746fb-115">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="746fb-116">A clonagem é uma operação de longa duração.</span><span class="sxs-lookup"><span data-stu-id="746fb-116">Cloning is a long-running operation.</span></span>
<span data-ttu-id="746fb-117">Depois que o clone POST retorna, você precisa OBTER a operação retornada pelo header Location: para ver se ele está "em execução" ou "bem-sucedido" ou "falhou". [](../resources/teamsasyncoperation.md)</span><span class="sxs-lookup"><span data-stu-id="746fb-117">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) returned by the Location: header to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="746fb-118">Você deve continuar a OBTER até que o status não seja "em execução".</span><span class="sxs-lookup"><span data-stu-id="746fb-118">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="746fb-119">O atraso recomendado entre GETs é de 5 segundos.</span><span class="sxs-lookup"><span data-stu-id="746fb-119">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="746fb-120">Permissions</span><span class="sxs-lookup"><span data-stu-id="746fb-120">Permissions</span></span>

<span data-ttu-id="746fb-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="746fb-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="746fb-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="746fb-123">Permission type</span></span>      | <span data-ttu-id="746fb-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="746fb-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="746fb-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="746fb-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="746fb-126">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="746fb-126">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="746fb-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="746fb-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="746fb-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="746fb-128">Not supported.</span></span>    |
|<span data-ttu-id="746fb-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="746fb-129">Application</span></span>                            | <span data-ttu-id="746fb-130">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="746fb-130">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="746fb-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="746fb-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="746fb-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="746fb-132">Request headers</span></span>
| <span data-ttu-id="746fb-133">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="746fb-133">Header</span></span>       | <span data-ttu-id="746fb-134">Valor</span><span class="sxs-lookup"><span data-stu-id="746fb-134">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="746fb-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="746fb-135">Authorization</span></span>  | <span data-ttu-id="746fb-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="746fb-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="746fb-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="746fb-138">Content-Type</span></span>  | <span data-ttu-id="746fb-139">application/json</span><span class="sxs-lookup"><span data-stu-id="746fb-139">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="746fb-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="746fb-140">Request body</span></span>

| <span data-ttu-id="746fb-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="746fb-141">Property</span></span>     | <span data-ttu-id="746fb-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="746fb-142">Type</span></span>   |<span data-ttu-id="746fb-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="746fb-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="746fb-144">classificação</span><span class="sxs-lookup"><span data-stu-id="746fb-144">classification</span></span>|<span data-ttu-id="746fb-145">Cadeia de caracteres (opcional)</span><span class="sxs-lookup"><span data-stu-id="746fb-145">String (optional)</span></span>|<span data-ttu-id="746fb-146">Descreve uma classificação para o grupo (como baixo, médio ou alto impacto comercial).</span><span class="sxs-lookup"><span data-stu-id="746fb-146">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="746fb-147">Os valores válidos para essa propriedade são definidos criando um valor de configuração [ClassificationList,](../resources/directorysetting.md) com base na [definição do modelo](../resources/directorysettingtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="746fb-147">Valid values for this property are defined by creating a ClassificationList [setting](../resources/directorysetting.md) value, based on the [template definition](../resources/directorysettingtemplate.md).</span></span> <span data-ttu-id="746fb-148">Se a classificação não for especificada, a classificação será copiada da equipe/grupo original.</span><span class="sxs-lookup"><span data-stu-id="746fb-148">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="746fb-149">description</span><span class="sxs-lookup"><span data-stu-id="746fb-149">description</span></span>|<span data-ttu-id="746fb-150">Cadeia de caracteres (opcional)</span><span class="sxs-lookup"><span data-stu-id="746fb-150">String (optional)</span></span>|<span data-ttu-id="746fb-151">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="746fb-151">An optional description for the group.</span></span> <span data-ttu-id="746fb-152">Se essa propriedade não for especificada, ela ficará em branco.</span><span class="sxs-lookup"><span data-stu-id="746fb-152">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="746fb-153">displayName</span><span class="sxs-lookup"><span data-stu-id="746fb-153">displayName</span></span>|<span data-ttu-id="746fb-154">String</span><span class="sxs-lookup"><span data-stu-id="746fb-154">String</span></span>|<span data-ttu-id="746fb-p109">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="746fb-p109">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="746fb-158">mailNickname</span><span class="sxs-lookup"><span data-stu-id="746fb-158">mailNickname</span></span>|<span data-ttu-id="746fb-159">String</span><span class="sxs-lookup"><span data-stu-id="746fb-159">String</span></span>|<span data-ttu-id="746fb-160">O alias de email do grupo, exclusivo na organização.</span><span class="sxs-lookup"><span data-stu-id="746fb-160">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="746fb-161">Essa propriedade deve ser especificada quando um grupo é criado.</span><span class="sxs-lookup"><span data-stu-id="746fb-161">This property must be specified when a group is created.</span></span> <span data-ttu-id="746fb-162">Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="746fb-162">Supports $filter.</span></span> <span data-ttu-id="746fb-163">Se essa propriedade não for especificada, ela será calculada a partir do displayName.</span><span class="sxs-lookup"><span data-stu-id="746fb-163">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="746fb-164">Problema conhecido: essa propriedade é ignorada no momento.</span><span class="sxs-lookup"><span data-stu-id="746fb-164">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="746fb-165">partsToClone</span><span class="sxs-lookup"><span data-stu-id="746fb-165">partsToClone</span></span>| [<span data-ttu-id="746fb-166">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="746fb-166">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="746fb-167">Uma lista separada por vírgulas das partes a ser clonada.</span><span class="sxs-lookup"><span data-stu-id="746fb-167">A comma-separated list of the parts to clone.</span></span> <span data-ttu-id="746fb-168">As partes legais são "aplicativos, guias, configurações, canais, membros".</span><span class="sxs-lookup"><span data-stu-id="746fb-168">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="746fb-169">visibility</span><span class="sxs-lookup"><span data-stu-id="746fb-169">visibility</span></span>|<span data-ttu-id="746fb-170">[teamVisibilityType](../resources/teamvisibilitytype.md) (opcional)</span><span class="sxs-lookup"><span data-stu-id="746fb-170">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="746fb-171">Especifica a visibilidade do grupo.</span><span class="sxs-lookup"><span data-stu-id="746fb-171">Specifies the visibility of the group.</span></span> <span data-ttu-id="746fb-172">Os valores possíveis são: **Private**, **Public**.</span><span class="sxs-lookup"><span data-stu-id="746fb-172">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="746fb-173">Se a visibilidade não for especificada, a visibilidade será copiada da equipe/grupo original.</span><span class="sxs-lookup"><span data-stu-id="746fb-173">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="746fb-174">Se a equipe que está sendo clonada for uma equipe **educationClass,** o parâmetro de visibilidade será ignorado e a visibilidade do novo grupo será definida como HiddenMembership.</span><span class="sxs-lookup"><span data-stu-id="746fb-174">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="746fb-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="746fb-175">Response</span></span>

<span data-ttu-id="746fb-176">Se tiver êxito, este método retornará um código `202 Accepted` de resposta com um header Location: apontando para o recurso [de](../resources/teamsasyncoperation.md) operação.</span><span class="sxs-lookup"><span data-stu-id="746fb-176">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="746fb-177">Quando a operação for concluída, o recurso de operação dirá a id da equipe criada.</span><span class="sxs-lookup"><span data-stu-id="746fb-177">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="746fb-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="746fb-178">Example</span></span>
#### <a name="request"></a><span data-ttu-id="746fb-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="746fb-179">Request</span></span>
<span data-ttu-id="746fb-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="746fb-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="746fb-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="746fb-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="746fb-182">C#</span><span class="sxs-lookup"><span data-stu-id="746fb-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/clone-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="746fb-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="746fb-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/clone-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="746fb-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="746fb-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/clone-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="746fb-185">Java</span><span class="sxs-lookup"><span data-stu-id="746fb-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/clone-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="746fb-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="746fb-186">Response</span></span>
<span data-ttu-id="746fb-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="746fb-187">The following is an example of the response.</span></span> <span data-ttu-id="746fb-188">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="746fb-188">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


