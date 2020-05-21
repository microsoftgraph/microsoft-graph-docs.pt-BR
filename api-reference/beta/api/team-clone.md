---
title: Clonar uma equipe
description: Criar uma cópia de uma equipe. Essa operação também cria uma cópia do grupo correspondente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bfda3767fc8c9bec58d78efc566efcfdf1b51c17
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332457"
---
# <a name="clone-a-team"></a><span data-ttu-id="016e3-104">Clonar uma equipe</span><span class="sxs-lookup"><span data-stu-id="016e3-104">Clone a team</span></span>

<span data-ttu-id="016e3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="016e3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="016e3-106">Criar uma cópia de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="016e3-106">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="016e3-107">Essa operação também cria uma cópia do [grupo](../resources/group.md)correspondente.</span><span class="sxs-lookup"><span data-stu-id="016e3-107">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="016e3-108">Você pode especificar quais partes da equipe serão clonadas:</span><span class="sxs-lookup"><span data-stu-id="016e3-108">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="016e3-109">**aplicativos** – copia os aplicativos do Microsoft Teams instalados na equipe.</span><span class="sxs-lookup"><span data-stu-id="016e3-109">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="016e3-110">**canais** – copia a estrutura do canal (mas não as mensagens no canal).</span><span class="sxs-lookup"><span data-stu-id="016e3-110">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="016e3-111">**Membros** – copia os membros e os proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="016e3-111">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="016e3-112">**configurações** – copia Todas as configurações da equipe, juntamente com as configurações de grupo de chaves.</span><span class="sxs-lookup"><span data-stu-id="016e3-112">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="016e3-113">**guias** – copia as guias nos canais.</span><span class="sxs-lookup"><span data-stu-id="016e3-113">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="016e3-114">Quando as guias são clonadas, elas são colocadas em um estado não configurado – elas são exibidas na barra de guias do Microsoft Teams e na primeira vez que você as abre, você passará pela tela de configuração.</span><span class="sxs-lookup"><span data-stu-id="016e3-114">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="016e3-115">(Se a pessoa que estiver abrindo a guia não tiver permissão para configurar aplicativos, verá uma mensagem explicando que a guia não foi configurada.)</span><span class="sxs-lookup"><span data-stu-id="016e3-115">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="016e3-116">A clonagem é uma operação de execução demorada.</span><span class="sxs-lookup"><span data-stu-id="016e3-116">Cloning is a long-running operation.</span></span>
<span data-ttu-id="016e3-117">Depois que o clone pós retornar, você precisará obter a [operação](../resources/teamsasyncoperation.md) retornada pelo cabeçalho Location: para ver se ele está "em execução" ou "bem-sucedido" ou "com falha".</span><span class="sxs-lookup"><span data-stu-id="016e3-117">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) returned by the Location: header to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="016e3-118">Você deve continuar a obter até que o status não seja "em execução".</span><span class="sxs-lookup"><span data-stu-id="016e3-118">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="016e3-119">O atraso recomendado entre GETs é de 5 segundos.</span><span class="sxs-lookup"><span data-stu-id="016e3-119">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="016e3-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="016e3-120">Permissions</span></span>

<span data-ttu-id="016e3-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="016e3-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="016e3-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="016e3-123">Permission type</span></span>      | <span data-ttu-id="016e3-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="016e3-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="016e3-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="016e3-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="016e3-126">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="016e3-126">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="016e3-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="016e3-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="016e3-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="016e3-128">Not supported.</span></span>    |
|<span data-ttu-id="016e3-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="016e3-129">Application</span></span>                            | <span data-ttu-id="016e3-130">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="016e3-130">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="016e3-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="016e3-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="016e3-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="016e3-132">Request headers</span></span>
| <span data-ttu-id="016e3-133">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="016e3-133">Header</span></span>       | <span data-ttu-id="016e3-134">Valor</span><span class="sxs-lookup"><span data-stu-id="016e3-134">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="016e3-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="016e3-135">Authorization</span></span>  | <span data-ttu-id="016e3-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="016e3-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="016e3-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="016e3-138">Content-Type</span></span>  | <span data-ttu-id="016e3-139">application/json</span><span class="sxs-lookup"><span data-stu-id="016e3-139">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="016e3-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="016e3-140">Request body</span></span>

| <span data-ttu-id="016e3-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="016e3-141">Property</span></span>     | <span data-ttu-id="016e3-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="016e3-142">Type</span></span>   |<span data-ttu-id="016e3-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="016e3-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="016e3-144">classificação</span><span class="sxs-lookup"><span data-stu-id="016e3-144">classification</span></span>|<span data-ttu-id="016e3-145">Cadeia de caracteres (opcional)</span><span class="sxs-lookup"><span data-stu-id="016e3-145">String (optional)</span></span>|<span data-ttu-id="016e3-146">Descreve uma classificação para o grupo (como impacto comercial baixo, médio ou alto).</span><span class="sxs-lookup"><span data-stu-id="016e3-146">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="016e3-147">Os valores válidos para essa propriedade são definidos pela criação de um valor de [configuração](../resources/directorysetting.md) de classificação, com base na [definição de modelo](../resources/directorysettingtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="016e3-147">Valid values for this property are defined by creating a ClassificationList [setting](../resources/directorysetting.md) value, based on the [template definition](../resources/directorysettingtemplate.md).</span></span> <span data-ttu-id="016e3-148">Se a classificação não for especificada, a classificação será copiada da equipe/grupo original.</span><span class="sxs-lookup"><span data-stu-id="016e3-148">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="016e3-149">description</span><span class="sxs-lookup"><span data-stu-id="016e3-149">description</span></span>|<span data-ttu-id="016e3-150">Cadeia de caracteres (opcional)</span><span class="sxs-lookup"><span data-stu-id="016e3-150">String (optional)</span></span>|<span data-ttu-id="016e3-151">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="016e3-151">An optional description for the group.</span></span> <span data-ttu-id="016e3-152">Se essa propriedade não for especificada, será deixada em branco.</span><span class="sxs-lookup"><span data-stu-id="016e3-152">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="016e3-153">displayName</span><span class="sxs-lookup"><span data-stu-id="016e3-153">displayName</span></span>|<span data-ttu-id="016e3-154">String</span><span class="sxs-lookup"><span data-stu-id="016e3-154">String</span></span>|<span data-ttu-id="016e3-p109">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="016e3-p109">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="016e3-158">mailNickname</span><span class="sxs-lookup"><span data-stu-id="016e3-158">mailNickname</span></span>|<span data-ttu-id="016e3-159">String</span><span class="sxs-lookup"><span data-stu-id="016e3-159">String</span></span>|<span data-ttu-id="016e3-160">O alias de email do grupo, exclusivo na organização.</span><span class="sxs-lookup"><span data-stu-id="016e3-160">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="016e3-161">Essa propriedade deve ser especificada quando um grupo é criado.</span><span class="sxs-lookup"><span data-stu-id="016e3-161">This property must be specified when a group is created.</span></span> <span data-ttu-id="016e3-162">Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="016e3-162">Supports $filter.</span></span> <span data-ttu-id="016e3-163">Se essa propriedade não for especificada, será calculada a partir do displayName.</span><span class="sxs-lookup"><span data-stu-id="016e3-163">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="016e3-164">Problema conhecido: esta propriedade é ignorada no momento.</span><span class="sxs-lookup"><span data-stu-id="016e3-164">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="016e3-165">partsToClone</span><span class="sxs-lookup"><span data-stu-id="016e3-165">partsToClone</span></span>| [<span data-ttu-id="016e3-166">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="016e3-166">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="016e3-167">Uma lista separada por vírgulas das partes a serem clonadas.</span><span class="sxs-lookup"><span data-stu-id="016e3-167">A comma-separated list of the parts to clone.</span></span> <span data-ttu-id="016e3-168">As partes legais são "aplicativos, guias, configurações, canais, membros".</span><span class="sxs-lookup"><span data-stu-id="016e3-168">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="016e3-169">visibility</span><span class="sxs-lookup"><span data-stu-id="016e3-169">visibility</span></span>|<span data-ttu-id="016e3-170">[teamVisibilityType](../resources/teamvisibilitytype.md) (opcional)</span><span class="sxs-lookup"><span data-stu-id="016e3-170">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="016e3-171">Especifica a visibilidade do grupo.</span><span class="sxs-lookup"><span data-stu-id="016e3-171">Specifies the visibility of the group.</span></span> <span data-ttu-id="016e3-172">Os valores possíveis são: **Private**, **Public**.</span><span class="sxs-lookup"><span data-stu-id="016e3-172">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="016e3-173">Se a visibilidade não for especificada, a visibilidade será copiada da equipe/grupo original.</span><span class="sxs-lookup"><span data-stu-id="016e3-173">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="016e3-174">Se a equipe que está sendo clonada for uma equipe do **educationClass** , o parâmetro Visibility será ignorado e a visibilidade do novo grupo será definida como HiddenMembership.</span><span class="sxs-lookup"><span data-stu-id="016e3-174">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="016e3-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="016e3-175">Response</span></span>

<span data-ttu-id="016e3-176">Se tiver êxito, este método retornará um `202 Accepted` código de resposta com um local: cabeçalho apontando para o recurso [Operation](../resources/teamsasyncoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="016e3-176">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="016e3-177">Quando a operação for concluída, o recurso de operação informará o ID da equipe criada.</span><span class="sxs-lookup"><span data-stu-id="016e3-177">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="016e3-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="016e3-178">Example</span></span>
#### <a name="request"></a><span data-ttu-id="016e3-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="016e3-179">Request</span></span>
<span data-ttu-id="016e3-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="016e3-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="016e3-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="016e3-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="016e3-182">C#</span><span class="sxs-lookup"><span data-stu-id="016e3-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/clone-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="016e3-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="016e3-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/clone-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="016e3-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="016e3-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/clone-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="016e3-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="016e3-185">Response</span></span>
<span data-ttu-id="016e3-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="016e3-186">The following is an example of the response.</span></span> <span data-ttu-id="016e3-187">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="016e3-187">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="016e3-188">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="016e3-188">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
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
