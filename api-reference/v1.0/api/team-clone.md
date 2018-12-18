---
title: Como clonar uma equipe
description: Crie uma cópia de uma equipe. Esta operação também cria uma cópia do grupo correspondente.
author: nkramer
ms.openlocfilehash: 21671ccbe440a57f6d745f9587c09b4432e25c35
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321830"
---
# <a name="clone-a-team"></a><span data-ttu-id="f7202-104">Como clonar uma equipe</span><span class="sxs-lookup"><span data-stu-id="f7202-104">Clone a team</span></span>



<span data-ttu-id="f7202-105">Crie uma cópia de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="f7202-105">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="f7202-106">Esta operação também cria uma cópia do [grupo](../resources/group.md)correspondente.</span><span class="sxs-lookup"><span data-stu-id="f7202-106">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="f7202-107">Você pode especificar quais partes da equipe a ser clonada:</span><span class="sxs-lookup"><span data-stu-id="f7202-107">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="f7202-108">**apps** - apps cópias equipes da Microsoft que estão instalados na equipe de.</span><span class="sxs-lookup"><span data-stu-id="f7202-108">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="f7202-109">**canais** – copia a estrutura de canal (mas não as mensagens no canal).</span><span class="sxs-lookup"><span data-stu-id="f7202-109">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="f7202-110">**membros** – copia os membros e proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="f7202-110">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="f7202-111">**configurações** – copia todas as definições dentro da equipe, juntamente com as configurações de chave de grupo.</span><span class="sxs-lookup"><span data-stu-id="f7202-111">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="f7202-112">**guias** – copia as guias no canais.</span><span class="sxs-lookup"><span data-stu-id="f7202-112">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="f7202-113">Quando as guias são clonados, eles são colocados em um estado não configurado- - são exibidas na barra de ferramentas guia da Microsoft Teams e, na primeira vez que você abri-los, vá através da tela de configuração.</span><span class="sxs-lookup"><span data-stu-id="f7202-113">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="f7202-114">(Se a pessoa que está abrindo a guia não tem permissão para configurar os aplicativos, eles verão uma mensagem que explica que a guia ainda não foram configurada.)</span><span class="sxs-lookup"><span data-stu-id="f7202-114">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="f7202-115">A clonagem é uma operação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="f7202-115">Cloning is a long-running operation.</span></span>
<span data-ttu-id="f7202-116">Depois que o clone POST retorna, você precisará fazer a [operação](../resources/teamsasyncoperation.md) para verificar se ele está "em execução" ou "sucedidas" ou "Falha".</span><span class="sxs-lookup"><span data-stu-id="f7202-116">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="f7202-117">Você deve continuar GET até que o status não é "executando".</span><span class="sxs-lookup"><span data-stu-id="f7202-117">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="f7202-118">O atraso recomendado entre obtém é 5 segundos.</span><span class="sxs-lookup"><span data-stu-id="f7202-118">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7202-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7202-119">Permissions</span></span>

<span data-ttu-id="f7202-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7202-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7202-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7202-122">Permission type</span></span>      | <span data-ttu-id="f7202-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7202-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7202-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7202-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7202-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7202-125">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7202-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7202-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7202-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7202-127">Not supported.</span></span>    |
|<span data-ttu-id="f7202-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7202-128">Application</span></span>                            | <span data-ttu-id="f7202-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7202-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7202-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7202-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="f7202-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7202-131">Request headers</span></span>
| <span data-ttu-id="f7202-132">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7202-132">Header</span></span>       | <span data-ttu-id="f7202-133">Valor</span><span class="sxs-lookup"><span data-stu-id="f7202-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f7202-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7202-134">Authorization</span></span>  | <span data-ttu-id="f7202-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7202-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f7202-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7202-137">Content-Type</span></span>  | <span data-ttu-id="f7202-138">application/json</span><span class="sxs-lookup"><span data-stu-id="f7202-138">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7202-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7202-139">Request body</span></span>

| <span data-ttu-id="f7202-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7202-140">Property</span></span>     | <span data-ttu-id="f7202-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7202-141">Type</span></span>   |<span data-ttu-id="f7202-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7202-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7202-143">classificação</span><span class="sxs-lookup"><span data-stu-id="f7202-143">classification</span></span>|<span data-ttu-id="f7202-144">Cadeia de caracteres (opcional)</span><span class="sxs-lookup"><span data-stu-id="f7202-144">String (optional)</span></span>|<span data-ttu-id="f7202-145">Descreve uma classificação para o grupo (por exemplo, o impacto comercial baixa, média ou alta).</span><span class="sxs-lookup"><span data-stu-id="f7202-145">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="f7202-146">Se a classificação não for especificada, a classificação será copiada do team/grupo original.</span><span class="sxs-lookup"><span data-stu-id="f7202-146">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="f7202-147">description</span><span class="sxs-lookup"><span data-stu-id="f7202-147">description</span></span>|<span data-ttu-id="f7202-148">Cadeia de caracteres (opcional)</span><span class="sxs-lookup"><span data-stu-id="f7202-148">String (optional)</span></span>|<span data-ttu-id="f7202-149">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="f7202-149">An optional description for the group.</span></span> <span data-ttu-id="f7202-150">Se essa propriedade não for especificada, ele será deixado em branco.</span><span class="sxs-lookup"><span data-stu-id="f7202-150">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="f7202-151">displayName</span><span class="sxs-lookup"><span data-stu-id="f7202-151">displayName</span></span>|<span data-ttu-id="f7202-152">String</span><span class="sxs-lookup"><span data-stu-id="f7202-152">String</span></span>|<span data-ttu-id="f7202-p109">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="f7202-p109">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="f7202-156">mailNickname</span><span class="sxs-lookup"><span data-stu-id="f7202-156">mailNickname</span></span>|<span data-ttu-id="f7202-157">String</span><span class="sxs-lookup"><span data-stu-id="f7202-157">String</span></span>|<span data-ttu-id="f7202-158">O alias de email para o grupo, exclusivo na organização.</span><span class="sxs-lookup"><span data-stu-id="f7202-158">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="f7202-159">Esta propriedade deve ser especificada quando um grupo é criado.</span><span class="sxs-lookup"><span data-stu-id="f7202-159">This property must be specified when a group is created.</span></span> <span data-ttu-id="f7202-160">Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="f7202-160">Supports $filter.</span></span> <span data-ttu-id="f7202-161">Se essa propriedade não for especificada, ele será calculado de displayName.</span><span class="sxs-lookup"><span data-stu-id="f7202-161">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="f7202-162">Problema conhecido: esta propriedade é ignorada no momento.</span><span class="sxs-lookup"><span data-stu-id="f7202-162">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="f7202-163">partsToClone</span><span class="sxs-lookup"><span data-stu-id="f7202-163">partsToClone</span></span>| [<span data-ttu-id="f7202-164">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="f7202-164">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="f7202-165">Uma lista separada por vírgulas das partes a ser clonada.</span><span class="sxs-lookup"><span data-stu-id="f7202-165">A comma-seperated list of the parts to clone.</span></span> <span data-ttu-id="f7202-166">Partes legais são "apps, guias, configurações, canais, membros".</span><span class="sxs-lookup"><span data-stu-id="f7202-166">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="f7202-167">visibilidade</span><span class="sxs-lookup"><span data-stu-id="f7202-167">visibility</span></span>|<span data-ttu-id="f7202-168">[teamVisibilityType](../resources/teamvisibilitytype.md) (opcional)</span><span class="sxs-lookup"><span data-stu-id="f7202-168">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="f7202-169">Especifica a visibilidade do grupo.</span><span class="sxs-lookup"><span data-stu-id="f7202-169">Specifies the visibility of the group.</span></span> <span data-ttu-id="f7202-170">Os valores possíveis são: **particular**e **público**.</span><span class="sxs-lookup"><span data-stu-id="f7202-170">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="f7202-171">Se a visibilidade não for especificada, será copiada a visibilidade do team/grupo original.</span><span class="sxs-lookup"><span data-stu-id="f7202-171">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="f7202-172">Se a equipe que está sendo clonado é uma equipe **educationClass** , o parâmetro visibilidade será ignorado e visibilidade do novo grupo será definida como HiddenMembership.</span><span class="sxs-lookup"><span data-stu-id="f7202-172">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="f7202-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7202-173">Response</span></span>

<span data-ttu-id="f7202-174">Se tiver êxito, este método retornará um `202 Accepted` código de resposta com um local: cabeçalho apontando para o recurso de [operação](../resources/teamsasyncoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="f7202-174">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="f7202-175">Quando a operação for concluída, o recurso de operação informará a id da equipe de criação.</span><span class="sxs-lookup"><span data-stu-id="f7202-175">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="f7202-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7202-176">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f7202-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7202-177">Request</span></span>
<span data-ttu-id="f7202-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7202-178">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="f7202-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7202-179">Response</span></span>
<span data-ttu-id="f7202-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f7202-180">The following is an example of the response.</span></span> <span data-ttu-id="f7202-181">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f7202-181">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f7202-182">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7202-182">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
