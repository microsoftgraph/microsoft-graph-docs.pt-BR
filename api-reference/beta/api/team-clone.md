---
title: Como clonar uma equipe
description: Crie uma cópia de uma equipe. Esta operação também cria uma cópia do grupo correspondente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5ef317d004e3355f9b40fc44232b7c594a3e45a7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526162"
---
# <a name="clone-a-team"></a><span data-ttu-id="92a89-104">Como clonar uma equipe</span><span class="sxs-lookup"><span data-stu-id="92a89-104">Clone a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92a89-105">Crie uma cópia de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="92a89-105">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="92a89-106">Esta operação também cria uma cópia do [grupo](../resources/group.md)correspondente.</span><span class="sxs-lookup"><span data-stu-id="92a89-106">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="92a89-107">Você pode especificar quais partes da equipe a ser clonada:</span><span class="sxs-lookup"><span data-stu-id="92a89-107">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="92a89-108">**apps** - apps cópias equipes da Microsoft que estão instalados na equipe de.</span><span class="sxs-lookup"><span data-stu-id="92a89-108">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="92a89-109">**canais** – copia a estrutura de canal (mas não as mensagens no canal).</span><span class="sxs-lookup"><span data-stu-id="92a89-109">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="92a89-110">**membros** – copia os membros e proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="92a89-110">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="92a89-111">**configurações** – copia todas as definições dentro da equipe, juntamente com as configurações de chave de grupo.</span><span class="sxs-lookup"><span data-stu-id="92a89-111">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="92a89-112">**guias** – copia as guias no canais.</span><span class="sxs-lookup"><span data-stu-id="92a89-112">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="92a89-113">Quando as guias são clonados, eles são colocados em um estado não configurado- - são exibidas na barra de ferramentas guia da Microsoft Teams e, na primeira vez que você abri-los, vá através da tela de configuração.</span><span class="sxs-lookup"><span data-stu-id="92a89-113">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="92a89-114">(Se a pessoa que está abrindo a guia não tem permissão para configurar os aplicativos, eles verão uma mensagem que explica que a guia ainda não foram configurada.)</span><span class="sxs-lookup"><span data-stu-id="92a89-114">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="92a89-115">A clonagem é uma operação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="92a89-115">Cloning is a long-running operation.</span></span>
<span data-ttu-id="92a89-116">Depois que o clone POST retorna, você precisará fazer a [operação](../resources/teamsasyncoperation.md) para verificar se ele está "em execução" ou "sucedidas" ou "Falha".</span><span class="sxs-lookup"><span data-stu-id="92a89-116">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="92a89-117">Você deve continuar GET até que o status não é "executando".</span><span class="sxs-lookup"><span data-stu-id="92a89-117">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="92a89-118">O atraso recomendado entre obtém é 5 segundos.</span><span class="sxs-lookup"><span data-stu-id="92a89-118">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="92a89-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="92a89-119">Permissions</span></span>

<span data-ttu-id="92a89-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92a89-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92a89-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92a89-122">Permission type</span></span>      | <span data-ttu-id="92a89-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92a89-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92a89-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92a89-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="92a89-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92a89-125">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="92a89-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92a89-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92a89-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92a89-127">Not supported.</span></span>    |
|<span data-ttu-id="92a89-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92a89-128">Application</span></span>                            | <span data-ttu-id="92a89-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92a89-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92a89-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92a89-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="92a89-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92a89-131">Request headers</span></span>
| <span data-ttu-id="92a89-132">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92a89-132">Header</span></span>       | <span data-ttu-id="92a89-133">Valor</span><span class="sxs-lookup"><span data-stu-id="92a89-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="92a89-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="92a89-134">Authorization</span></span>  | <span data-ttu-id="92a89-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92a89-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="92a89-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="92a89-137">Content-Type</span></span>  | <span data-ttu-id="92a89-138">application/json</span><span class="sxs-lookup"><span data-stu-id="92a89-138">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="92a89-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92a89-139">Request body</span></span>

| <span data-ttu-id="92a89-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92a89-140">Property</span></span>     | <span data-ttu-id="92a89-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="92a89-141">Type</span></span>   |<span data-ttu-id="92a89-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="92a89-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92a89-143">classificação</span><span class="sxs-lookup"><span data-stu-id="92a89-143">classification</span></span>|<span data-ttu-id="92a89-144">Cadeia de caracteres (opcional)</span><span class="sxs-lookup"><span data-stu-id="92a89-144">String (optional)</span></span>|<span data-ttu-id="92a89-145">Descreve uma classificação para o grupo (por exemplo, o impacto comercial baixa, média ou alta).</span><span class="sxs-lookup"><span data-stu-id="92a89-145">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="92a89-146">Os valores válidos para essa propriedade são definidos com a criação de um valor de [configuração](../resources/directorysetting.md) de ClassificationList, com base na [definição de modelo](../resources/directorysettingtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="92a89-146">Valid values for this property are defined by creating a ClassificationList [setting](../resources/directorysetting.md) value, based on the [template definition](../resources/directorysettingtemplate.md).</span></span> <span data-ttu-id="92a89-147">Se a classificação não for especificada, a classificação será copiada do team/grupo original.</span><span class="sxs-lookup"><span data-stu-id="92a89-147">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="92a89-148">description</span><span class="sxs-lookup"><span data-stu-id="92a89-148">description</span></span>|<span data-ttu-id="92a89-149">Cadeia de caracteres (opcional)</span><span class="sxs-lookup"><span data-stu-id="92a89-149">String (optional)</span></span>|<span data-ttu-id="92a89-150">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="92a89-150">An optional description for the group.</span></span> <span data-ttu-id="92a89-151">Se essa propriedade não for especificada, ele será deixado em branco.</span><span class="sxs-lookup"><span data-stu-id="92a89-151">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="92a89-152">displayName</span><span class="sxs-lookup"><span data-stu-id="92a89-152">displayName</span></span>|<span data-ttu-id="92a89-153">String</span><span class="sxs-lookup"><span data-stu-id="92a89-153">String</span></span>|<span data-ttu-id="92a89-p109">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="92a89-p109">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="92a89-157">mailNickname</span><span class="sxs-lookup"><span data-stu-id="92a89-157">mailNickname</span></span>|<span data-ttu-id="92a89-158">String</span><span class="sxs-lookup"><span data-stu-id="92a89-158">String</span></span>|<span data-ttu-id="92a89-159">O alias de email do grupo, exclusivo na organização.</span><span class="sxs-lookup"><span data-stu-id="92a89-159">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="92a89-160">Essa propriedade deve ser especificada quando um grupo é criado.</span><span class="sxs-lookup"><span data-stu-id="92a89-160">This property must be specified when a group is created.</span></span> <span data-ttu-id="92a89-161">Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="92a89-161">Supports $filter.</span></span> <span data-ttu-id="92a89-162">Se essa propriedade não for especificada, ele será calculado de displayName.</span><span class="sxs-lookup"><span data-stu-id="92a89-162">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="92a89-163">Problema conhecido: esta propriedade é ignorada no momento.</span><span class="sxs-lookup"><span data-stu-id="92a89-163">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="92a89-164">partsToClone</span><span class="sxs-lookup"><span data-stu-id="92a89-164">partsToClone</span></span>| [<span data-ttu-id="92a89-165">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="92a89-165">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="92a89-166">Uma lista separada por vírgulas das partes a ser clonada.</span><span class="sxs-lookup"><span data-stu-id="92a89-166">A comma-seperated list of the parts to clone.</span></span> <span data-ttu-id="92a89-167">Partes legais são "apps, guias, configurações, canais, membros".</span><span class="sxs-lookup"><span data-stu-id="92a89-167">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="92a89-168">visibility</span><span class="sxs-lookup"><span data-stu-id="92a89-168">visibility</span></span>|<span data-ttu-id="92a89-169">[teamVisibilityType](../resources/teamvisibilitytype.md) (opcional)</span><span class="sxs-lookup"><span data-stu-id="92a89-169">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="92a89-170">Especifica a visibilidade do grupo.</span><span class="sxs-lookup"><span data-stu-id="92a89-170">Specifies the visibility of the group.</span></span> <span data-ttu-id="92a89-171">Os valores possíveis são: **particular**e **público**.</span><span class="sxs-lookup"><span data-stu-id="92a89-171">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="92a89-172">Se a visibilidade não for especificada, será copiada a visibilidade do team/grupo original.</span><span class="sxs-lookup"><span data-stu-id="92a89-172">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="92a89-173">Se a equipe que está sendo clonado é uma equipe **educationClass** , o parâmetro visibilidade será ignorado e visibilidade do novo grupo será definida como HiddenMembership.</span><span class="sxs-lookup"><span data-stu-id="92a89-173">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="92a89-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="92a89-174">Response</span></span>

<span data-ttu-id="92a89-175">Se tiver êxito, este método retornará um `202 Accepted` código de resposta com um local: cabeçalho apontando para o recurso de [operação](../resources/teamsasyncoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="92a89-175">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="92a89-176">Quando a operação for concluída, o recurso de operação informará a id da equipe de criação.</span><span class="sxs-lookup"><span data-stu-id="92a89-176">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="92a89-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92a89-177">Example</span></span>
#### <a name="request"></a><span data-ttu-id="92a89-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92a89-178">Request</span></span>
<span data-ttu-id="92a89-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="92a89-179">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
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

#### <a name="response"></a><span data-ttu-id="92a89-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="92a89-180">Response</span></span>
<span data-ttu-id="92a89-181">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="92a89-181">The following is an example of the response.</span></span> <span data-ttu-id="92a89-182">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="92a89-182">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="92a89-183">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92a89-183">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
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
  "suppressions": [
    "Error: /api-reference/beta/api/team-clone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
