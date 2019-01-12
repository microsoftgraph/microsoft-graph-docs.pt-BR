---
title: Como clonar uma equipe
description: Crie uma cópia de uma equipe. Esta operação também cria uma cópia do grupo correspondente.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4fb3769db0df6d2fc30d995098daee19b49e83b7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958338"
---
# <a name="clone-a-team"></a><span data-ttu-id="2020d-104">Como clonar uma equipe</span><span class="sxs-lookup"><span data-stu-id="2020d-104">Clone a team</span></span>

> <span data-ttu-id="2020d-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2020d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2020d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2020d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2020d-107">Crie uma cópia de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="2020d-107">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="2020d-108">Esta operação também cria uma cópia do [grupo](../resources/group.md)correspondente.</span><span class="sxs-lookup"><span data-stu-id="2020d-108">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="2020d-109">Você pode especificar quais partes da equipe a ser clonada:</span><span class="sxs-lookup"><span data-stu-id="2020d-109">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="2020d-110">**apps** - apps cópias equipes da Microsoft que estão instalados na equipe de.</span><span class="sxs-lookup"><span data-stu-id="2020d-110">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="2020d-111">**canais** – copia a estrutura de canal (mas não as mensagens no canal).</span><span class="sxs-lookup"><span data-stu-id="2020d-111">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="2020d-112">**membros** – copia os membros e proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="2020d-112">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="2020d-113">**configurações** – copia todas as definições dentro da equipe, juntamente com as configurações de chave de grupo.</span><span class="sxs-lookup"><span data-stu-id="2020d-113">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="2020d-114">**guias** – copia as guias no canais.</span><span class="sxs-lookup"><span data-stu-id="2020d-114">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="2020d-115">Quando as guias são clonados, eles são colocados em um estado não configurado- - são exibidas na barra de ferramentas guia da Microsoft Teams e, na primeira vez que você abri-los, vá através da tela de configuração.</span><span class="sxs-lookup"><span data-stu-id="2020d-115">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="2020d-116">(Se a pessoa que está abrindo a guia não tem permissão para configurar os aplicativos, eles verão uma mensagem que explica que a guia ainda não foram configurada.)</span><span class="sxs-lookup"><span data-stu-id="2020d-116">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="2020d-117">A clonagem é uma operação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="2020d-117">Cloning is a long-running operation.</span></span>
<span data-ttu-id="2020d-118">Depois que o clone POST retorna, você precisará fazer a [operação](../resources/teamsasyncoperation.md) para verificar se ele está "em execução" ou "sucedidas" ou "Falha".</span><span class="sxs-lookup"><span data-stu-id="2020d-118">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="2020d-119">Você deve continuar GET até que o status não é "executando".</span><span class="sxs-lookup"><span data-stu-id="2020d-119">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="2020d-120">O atraso recomendado entre obtém é 5 segundos.</span><span class="sxs-lookup"><span data-stu-id="2020d-120">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="2020d-121">Permissions</span><span class="sxs-lookup"><span data-stu-id="2020d-121">Permissions</span></span>

<span data-ttu-id="2020d-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2020d-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2020d-124">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2020d-124">Permission type</span></span>      | <span data-ttu-id="2020d-125">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2020d-125">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2020d-126">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2020d-126">Delegated (work or school account)</span></span>     | <span data-ttu-id="2020d-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2020d-127">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2020d-128">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2020d-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2020d-129">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2020d-129">Not supported.</span></span>    |
|<span data-ttu-id="2020d-130">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2020d-130">Application</span></span>                            | <span data-ttu-id="2020d-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2020d-131">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2020d-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2020d-132">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="2020d-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2020d-133">Request headers</span></span>
| <span data-ttu-id="2020d-134">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2020d-134">Header</span></span>       | <span data-ttu-id="2020d-135">Valor</span><span class="sxs-lookup"><span data-stu-id="2020d-135">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2020d-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="2020d-136">Authorization</span></span>  | <span data-ttu-id="2020d-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2020d-p107">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2020d-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2020d-139">Content-Type</span></span>  | <span data-ttu-id="2020d-140">application/json</span><span class="sxs-lookup"><span data-stu-id="2020d-140">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2020d-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2020d-141">Request body</span></span>

| <span data-ttu-id="2020d-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2020d-142">Property</span></span>     | <span data-ttu-id="2020d-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="2020d-143">Type</span></span>   |<span data-ttu-id="2020d-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="2020d-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2020d-145">classificação</span><span class="sxs-lookup"><span data-stu-id="2020d-145">classification</span></span>|<span data-ttu-id="2020d-146">Cadeia de caracteres (opcional)</span><span class="sxs-lookup"><span data-stu-id="2020d-146">String (optional)</span></span>|<span data-ttu-id="2020d-147">Descreve uma classificação para o grupo (por exemplo, o impacto comercial baixa, média ou alta).</span><span class="sxs-lookup"><span data-stu-id="2020d-147">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="2020d-148">Os valores válidos para essa propriedade são definidos com a criação de um valor de [configuração](../resources/directorysetting.md) de ClassificationList, com base na [definição de modelo](../resources/directorysettingtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="2020d-148">Valid values for this property are defined by creating a ClassificationList [setting](../resources/directorysetting.md) value, based on the [template definition](../resources/directorysettingtemplate.md).</span></span> <span data-ttu-id="2020d-149">Se a classificação não for especificada, a classificação será copiada do team/grupo original.</span><span class="sxs-lookup"><span data-stu-id="2020d-149">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="2020d-150">description</span><span class="sxs-lookup"><span data-stu-id="2020d-150">description</span></span>|<span data-ttu-id="2020d-151">Cadeia de caracteres (opcional)</span><span class="sxs-lookup"><span data-stu-id="2020d-151">String (optional)</span></span>|<span data-ttu-id="2020d-152">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="2020d-152">An optional description for the group.</span></span> <span data-ttu-id="2020d-153">Se essa propriedade não for especificada, ele será deixado em branco.</span><span class="sxs-lookup"><span data-stu-id="2020d-153">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="2020d-154">displayName</span><span class="sxs-lookup"><span data-stu-id="2020d-154">displayName</span></span>|<span data-ttu-id="2020d-155">String</span><span class="sxs-lookup"><span data-stu-id="2020d-155">String</span></span>|<span data-ttu-id="2020d-p110">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="2020d-p110">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="2020d-159">mailNickname</span><span class="sxs-lookup"><span data-stu-id="2020d-159">mailNickname</span></span>|<span data-ttu-id="2020d-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2020d-160">String</span></span>|<span data-ttu-id="2020d-161">O alias de email para o grupo, exclusivo na organização.</span><span class="sxs-lookup"><span data-stu-id="2020d-161">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="2020d-162">Esta propriedade deve ser especificada quando um grupo é criado.</span><span class="sxs-lookup"><span data-stu-id="2020d-162">This property must be specified when a group is created.</span></span> <span data-ttu-id="2020d-163">Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="2020d-163">Supports $filter.</span></span> <span data-ttu-id="2020d-164">Se essa propriedade não for especificada, ele será calculado de displayName.</span><span class="sxs-lookup"><span data-stu-id="2020d-164">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="2020d-165">Problema conhecido: esta propriedade é ignorada no momento.</span><span class="sxs-lookup"><span data-stu-id="2020d-165">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="2020d-166">partsToClone</span><span class="sxs-lookup"><span data-stu-id="2020d-166">partsToClone</span></span>| [<span data-ttu-id="2020d-167">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="2020d-167">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="2020d-168">Uma lista separada por vírgulas das partes a ser clonada.</span><span class="sxs-lookup"><span data-stu-id="2020d-168">A comma-seperated list of the parts to clone.</span></span> <span data-ttu-id="2020d-169">Partes legais são "apps, guias, configurações, canais, membros".</span><span class="sxs-lookup"><span data-stu-id="2020d-169">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="2020d-170">visibilidade</span><span class="sxs-lookup"><span data-stu-id="2020d-170">visibility</span></span>|<span data-ttu-id="2020d-171">[teamVisibilityType](../resources/teamvisibilitytype.md) (opcional)</span><span class="sxs-lookup"><span data-stu-id="2020d-171">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="2020d-172">Especifica a visibilidade do grupo.</span><span class="sxs-lookup"><span data-stu-id="2020d-172">Specifies the visibility of the group.</span></span> <span data-ttu-id="2020d-173">Os valores possíveis são: **particular**e **público**.</span><span class="sxs-lookup"><span data-stu-id="2020d-173">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="2020d-174">Se a visibilidade não for especificada, será copiada a visibilidade do team/grupo original.</span><span class="sxs-lookup"><span data-stu-id="2020d-174">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="2020d-175">Se a equipe que está sendo clonado é uma equipe **educationClass** , o parâmetro visibilidade será ignorado e visibilidade do novo grupo será definida como HiddenMembership.</span><span class="sxs-lookup"><span data-stu-id="2020d-175">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="2020d-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="2020d-176">Response</span></span>

<span data-ttu-id="2020d-177">Se tiver êxito, este método retornará um `202 Accepted` código de resposta com um local: cabeçalho apontando para o recurso de [operação](../resources/teamsasyncoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="2020d-177">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="2020d-178">Quando a operação for concluída, o recurso de operação informará a id da equipe de criação.</span><span class="sxs-lookup"><span data-stu-id="2020d-178">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="2020d-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2020d-179">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2020d-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2020d-180">Request</span></span>
<span data-ttu-id="2020d-181">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2020d-181">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="2020d-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="2020d-182">Response</span></span>
<span data-ttu-id="2020d-183">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2020d-183">The following is an example of the response.</span></span> <span data-ttu-id="2020d-184">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="2020d-184">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2020d-185">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2020d-185">All of the properties will be returned from an actual call.</span></span>
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
