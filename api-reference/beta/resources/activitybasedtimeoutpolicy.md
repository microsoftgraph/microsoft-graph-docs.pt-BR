---
title: Tipo de recurso activityBasedTimeoutPolicy
description: Representa uma política que pode controlar o tempo de inativo para sessões da Web para aplicativos que suportam a funcionalidade de tempo de tempo de atividade baseada em atividade.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 62f18c7083f96abd7d1cf1d2840aa4e29ce66554
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155591"
---
# <a name="activitybasedtimeoutpolicy-resource-type"></a><span data-ttu-id="69dea-103">Tipo de recurso activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="69dea-103">activityBasedTimeoutPolicy resource type</span></span>

<span data-ttu-id="69dea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69dea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69dea-105">Representa uma política que pode controlar o tempo de inativo para sessões da Web para aplicativos que suportam a funcionalidade de tempo de tempo de atividade baseada em atividade.</span><span class="sxs-lookup"><span data-stu-id="69dea-105">Represents a policy that can control the idle timeout for web sessions for applications that support activity-based timeout functionality.</span></span> <span data-ttu-id="69dea-106">Os aplicativos impõem a inscrição automática após um período de inatividade.</span><span class="sxs-lookup"><span data-stu-id="69dea-106">Applications enforce automatic signout after a period of inactivity.</span></span> <span data-ttu-id="69dea-107">Esse tipo de política só pode ser aplicado no nível da organização (definindo a **propriedade isOrganizationDefault** como `true` ).</span><span class="sxs-lookup"><span data-stu-id="69dea-107">This type of policy can only be applied at the organization level (by setting the **isOrganizationDefault** property to `true`).</span></span>

<span data-ttu-id="69dea-108">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="69dea-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="69dea-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="69dea-109">Methods</span></span>

| <span data-ttu-id="69dea-110">Método</span><span class="sxs-lookup"><span data-stu-id="69dea-110">Method</span></span>       | <span data-ttu-id="69dea-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="69dea-111">Return Type</span></span> | <span data-ttu-id="69dea-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="69dea-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="69dea-113">Criar activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="69dea-113">Create activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-post-activitybasedtimeoutpolicies.md) | [<span data-ttu-id="69dea-114">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="69dea-114">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="69dea-115">Criar um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="69dea-115">Create an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="69dea-116">Obter activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="69dea-116">Get activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-get.md) | [<span data-ttu-id="69dea-117">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="69dea-117">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="69dea-118">Ler propriedades e relações de um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="69dea-118">Read properties and relationships of an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="69dea-119">Listar activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="69dea-119">List activityBasedTimeoutPolicies</span></span>](../api/activitybasedtimeoutpolicy-list.md) | [<span data-ttu-id="69dea-120">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="69dea-120">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="69dea-121">Leia as propriedades e os relacionamentos dos objetos activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="69dea-121">Read properties and relationships of activityBasedTimeoutPolicy objects.</span></span> |
| [<span data-ttu-id="69dea-122">Atualizar activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="69dea-122">Update activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-update.md) | <span data-ttu-id="69dea-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="69dea-123">None</span></span> | <span data-ttu-id="69dea-124">Atualize um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="69dea-124">Update an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="69dea-125">Excluir activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="69dea-125">Delete activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-delete.md) | <span data-ttu-id="69dea-126">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="69dea-126">None</span></span> | <span data-ttu-id="69dea-127">Exclua um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="69dea-127">Delete an activityBasedTimeoutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="69dea-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69dea-128">Properties</span></span>

| <span data-ttu-id="69dea-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69dea-129">Property</span></span>     | <span data-ttu-id="69dea-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="69dea-130">Type</span></span>        | <span data-ttu-id="69dea-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="69dea-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="69dea-132">id</span><span class="sxs-lookup"><span data-stu-id="69dea-132">id</span></span>|<span data-ttu-id="69dea-133">String</span><span class="sxs-lookup"><span data-stu-id="69dea-133">String</span></span>| <span data-ttu-id="69dea-134">Identificador exclusivo desta política.</span><span class="sxs-lookup"><span data-stu-id="69dea-134">Unique identifier for this policy.</span></span> <span data-ttu-id="69dea-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69dea-135">Read-only.</span></span>|
|<span data-ttu-id="69dea-136">definição</span><span class="sxs-lookup"><span data-stu-id="69dea-136">definition</span></span>|<span data-ttu-id="69dea-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="69dea-137">String collection</span></span>| <span data-ttu-id="69dea-138">Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política.</span><span class="sxs-lookup"><span data-stu-id="69dea-138">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="69dea-139">Veja abaixo para obter mais detalhes sobre o esquema JSON para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="69dea-139">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="69dea-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69dea-140">Required.</span></span>|
|<span data-ttu-id="69dea-141">description</span><span class="sxs-lookup"><span data-stu-id="69dea-141">description</span></span>|<span data-ttu-id="69dea-142">String</span><span class="sxs-lookup"><span data-stu-id="69dea-142">String</span></span>| <span data-ttu-id="69dea-143">Descrição desta política.</span><span class="sxs-lookup"><span data-stu-id="69dea-143">Description for this policy.</span></span>|
|<span data-ttu-id="69dea-144">displayName</span><span class="sxs-lookup"><span data-stu-id="69dea-144">displayName</span></span>|<span data-ttu-id="69dea-145">String</span><span class="sxs-lookup"><span data-stu-id="69dea-145">String</span></span>| <span data-ttu-id="69dea-146">Nome para exibição desta política.</span><span class="sxs-lookup"><span data-stu-id="69dea-146">Display name for this policy.</span></span> <span data-ttu-id="69dea-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69dea-147">Required.</span></span>|
|<span data-ttu-id="69dea-148">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="69dea-148">isOrganizationDefault</span></span>|<span data-ttu-id="69dea-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="69dea-149">Boolean</span></span>|<span data-ttu-id="69dea-150">Se definido como true, ativa essa política.</span><span class="sxs-lookup"><span data-stu-id="69dea-150">If set to true, activates this policy.</span></span> <span data-ttu-id="69dea-151">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="69dea-151">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="69dea-152">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="69dea-152">Optional, default value is false.</span></span>|


### <a name="properties-of-an-activity-based-timeout-policy-definition"></a><span data-ttu-id="69dea-153">Propriedades de uma definição de política de tempo de vida baseada em atividade</span><span class="sxs-lookup"><span data-stu-id="69dea-153">Properties of an activity-based timeout policy definition</span></span>
<span data-ttu-id="69dea-154">As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida baseada em atividade.</span><span class="sxs-lookup"><span data-stu-id="69dea-154">The properties below form the JSON object that represents an activity-based timeout policy.</span></span> <span data-ttu-id="69dea-155">Esse objeto JSON deve ser **convertido em uma cadeia de caracteres** com aspas que não devem ser inseridas na propriedade de **definição.**</span><span class="sxs-lookup"><span data-stu-id="69dea-155">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="69dea-156">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="69dea-156">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```json
{
  "definition":["{\"ActivityBasedTimeoutPolicy\":{\"Version\":1,\"ApplicationPolicies\":[{\"ApplicationId\":\"default\",\"WebSessionIdleTimeout\":\"01:00:00\"},{\"ApplicationId\":\"c44b4083-3bb0-49c1-b47d-974e53cbdf3c\",\"WebSessionIdleTimeout\":\"00:15:00\"}]}}"]
}
```

><span data-ttu-id="69dea-157">Observação: todas as durações de tempo nessas propriedades são especificadas no formato "dd.hh:mm:ss".</span><span class="sxs-lookup"><span data-stu-id="69dea-157">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="69dea-158">Observação: os valores máximos para propriedades anotadas em "dias" são 1 segundo a menos do número de dias anotado.</span><span class="sxs-lookup"><span data-stu-id="69dea-158">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="69dea-159">Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="69dea-159">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="69dea-160">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69dea-160">Property</span></span>     | <span data-ttu-id="69dea-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="69dea-161">Type</span></span>   |<span data-ttu-id="69dea-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="69dea-162">Description</span></span>|
|:-------------|:------|:---------|
|<span data-ttu-id="69dea-163">Versão</span><span class="sxs-lookup"><span data-stu-id="69dea-163">Version</span></span>|<span data-ttu-id="69dea-164">Inteiro</span><span class="sxs-lookup"><span data-stu-id="69dea-164">Integer</span></span>|<span data-ttu-id="69dea-165">Versão da política.</span><span class="sxs-lookup"><span data-stu-id="69dea-165">Policy version.</span></span> <span data-ttu-id="69dea-166">Valor definido de 1.</span><span class="sxs-lookup"><span data-stu-id="69dea-166">Set value of 1.</span></span> <span data-ttu-id="69dea-167">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69dea-167">Required.</span></span>|
|<span data-ttu-id="69dea-168">ApplicationPolicies</span><span class="sxs-lookup"><span data-stu-id="69dea-168">ApplicationPolicies</span></span>|<span data-ttu-id="69dea-169">Objeto JSON</span><span class="sxs-lookup"><span data-stu-id="69dea-169">JSON object</span></span>|<span data-ttu-id="69dea-170">Coleção de política de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="69dea-170">Collection of application policy.</span></span> <span data-ttu-id="69dea-171">Uma política de aplicativo é uma combinação de ApplicationId e WebSessionIdleTimeout:</span><span class="sxs-lookup"><span data-stu-id="69dea-171">An application policy, is a combination of an ApplicationId and a WebSessionIdleTimeout:</span></span> <br> <ul><li><span data-ttu-id="69dea-172">**ApplicationId**: valores permitidos:</span><span class="sxs-lookup"><span data-stu-id="69dea-172">**ApplicationId**: Allowed values:</span></span><ul><li> <span data-ttu-id="69dea-173">padrão: aplica a política a todos os aplicativos que suportam a funcionalidade de tempoout baseada em atividade, mas não têm substituição específica do aplicativo</span><span class="sxs-lookup"><span data-stu-id="69dea-173">default: applies the policy to all applications that support activity-based timeout functionality but do not have application-specific override</span></span></li><li> <span data-ttu-id="69dea-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c: aplica a política ao Portal do Azure</span><span class="sxs-lookup"><span data-stu-id="69dea-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c: applies the policy to the Azure Portal</span></span></li></ul></li><li><span data-ttu-id="69dea-175">**WebSessionIdleTimeout**: o período de inatividade do usuário após o qual a sessão da Web do usuário é considerada expirada.</span><span class="sxs-lookup"><span data-stu-id="69dea-175">**WebSessionIdleTimeout**: The period of user inactivity after which the user's web session is considered expired.</span></span> <span data-ttu-id="69dea-176">O valor mínimo é 5 minutos; o valor máximo é de 1 dia.</span><span class="sxs-lookup"><span data-stu-id="69dea-176">The minimum value is 5 minutes; the maximum value is 1 day.</span></span></li></ul> |


## <a name="relationships"></a><span data-ttu-id="69dea-177">Relações</span><span class="sxs-lookup"><span data-stu-id="69dea-177">Relationships</span></span>

<span data-ttu-id="69dea-178">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69dea-178">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69dea-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69dea-179">JSON representation</span></span>

<span data-ttu-id="69dea-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69dea-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activityBasedTimeoutPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

