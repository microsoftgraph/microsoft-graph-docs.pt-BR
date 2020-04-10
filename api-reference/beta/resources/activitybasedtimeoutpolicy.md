---
title: tipo de recurso activityBasedTimeoutPolicy
description: Representa uma política que pode controlar o tempo limite de ociosidade para sessões da Web para aplicativos que dão suporte à funcionalidade de tempo limite baseada na atividade.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c5dea57ad86ff0c9209f3f88fc4a922daa13d257
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218489"
---
# <a name="activitybasedtimeoutpolicy-resource-type"></a><span data-ttu-id="c8e9c-103">tipo de recurso activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="c8e9c-103">activityBasedTimeoutPolicy resource type</span></span>

<span data-ttu-id="c8e9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8e9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8e9c-105">Representa uma política que pode controlar o tempo limite de ociosidade para sessões da Web para aplicativos que dão suporte à funcionalidade de tempo limite baseada na atividade.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-105">Represents a policy that can control the idle timeout for web sessions for applications that support activity-based timeout functionality.</span></span> <span data-ttu-id="c8e9c-106">Os aplicativos impõem a desconexão automática após um período de inatividade.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-106">Applications enforce automatic signout after a period of inactivity.</span></span> <span data-ttu-id="c8e9c-107">Esse tipo de política só pode ser aplicado no nível da organização (Configurando **isOrganizationDefault** a propriedade isOrganizationDefault `true`para).</span><span class="sxs-lookup"><span data-stu-id="c8e9c-107">This type of policy can only be applied at the organization level (by setting the **isOrganizationDefault** property to `true`).</span></span>

<span data-ttu-id="c8e9c-108">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c8e9c-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c8e9c-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="c8e9c-109">Methods</span></span>

| <span data-ttu-id="c8e9c-110">Método</span><span class="sxs-lookup"><span data-stu-id="c8e9c-110">Method</span></span>       | <span data-ttu-id="c8e9c-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c8e9c-111">Return Type</span></span> | <span data-ttu-id="c8e9c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8e9c-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c8e9c-113">Criar activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="c8e9c-113">Create activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-post-activitybasedtimeoutpolicies.md) | [<span data-ttu-id="c8e9c-114">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="c8e9c-114">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="c8e9c-115">Criar um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-115">Create an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="c8e9c-116">Obter activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="c8e9c-116">Get activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-get.md) | [<span data-ttu-id="c8e9c-117">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="c8e9c-117">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="c8e9c-118">Ler propriedades e relações de um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-118">Read properties and relationships of an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="c8e9c-119">Listar activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="c8e9c-119">List activityBasedTimeoutPolicies</span></span>](../api/activitybasedtimeoutpolicy-list.md) | [<span data-ttu-id="c8e9c-120">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="c8e9c-120">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="c8e9c-121">Ler propriedades e relações de objetos activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-121">Read properties and relationships of activityBasedTimeoutPolicy objects.</span></span> |
| [<span data-ttu-id="c8e9c-122">Atualizar activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="c8e9c-122">Update activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-update.md) | <span data-ttu-id="c8e9c-123">None</span><span class="sxs-lookup"><span data-stu-id="c8e9c-123">None</span></span> | <span data-ttu-id="c8e9c-124">Atualize um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-124">Update an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="c8e9c-125">Excluir activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="c8e9c-125">Delete activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-delete.md) | <span data-ttu-id="c8e9c-126">None</span><span class="sxs-lookup"><span data-stu-id="c8e9c-126">None</span></span> | <span data-ttu-id="c8e9c-127">Excluir um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-127">Delete an activityBasedTimeoutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c8e9c-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8e9c-128">Properties</span></span>

| <span data-ttu-id="c8e9c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8e9c-129">Property</span></span>     | <span data-ttu-id="c8e9c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8e9c-130">Type</span></span>        | <span data-ttu-id="c8e9c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8e9c-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c8e9c-132">id</span><span class="sxs-lookup"><span data-stu-id="c8e9c-132">id</span></span>|<span data-ttu-id="c8e9c-133">String</span><span class="sxs-lookup"><span data-stu-id="c8e9c-133">String</span></span>| <span data-ttu-id="c8e9c-134">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-134">Unique identifier for this policy.</span></span> <span data-ttu-id="c8e9c-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-135">Read-only.</span></span>|
|<span data-ttu-id="c8e9c-136">definir</span><span class="sxs-lookup"><span data-stu-id="c8e9c-136">definition</span></span>|<span data-ttu-id="c8e9c-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8e9c-137">String collection</span></span>| <span data-ttu-id="c8e9c-138">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-138">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="c8e9c-139">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-139">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="c8e9c-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-140">Required.</span></span>|
|<span data-ttu-id="c8e9c-141">description</span><span class="sxs-lookup"><span data-stu-id="c8e9c-141">description</span></span>|<span data-ttu-id="c8e9c-142">String</span><span class="sxs-lookup"><span data-stu-id="c8e9c-142">String</span></span>| <span data-ttu-id="c8e9c-143">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-143">Description for this policy.</span></span>|
|<span data-ttu-id="c8e9c-144">displayName</span><span class="sxs-lookup"><span data-stu-id="c8e9c-144">displayName</span></span>|<span data-ttu-id="c8e9c-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8e9c-145">String</span></span>| <span data-ttu-id="c8e9c-146">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-146">Display name for this policy.</span></span> <span data-ttu-id="c8e9c-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-147">Required.</span></span>|
|<span data-ttu-id="c8e9c-148">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="c8e9c-148">isOrganizationDefault</span></span>|<span data-ttu-id="c8e9c-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8e9c-149">Boolean</span></span>|<span data-ttu-id="c8e9c-150">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-150">If set to true, activates this policy.</span></span> <span data-ttu-id="c8e9c-151">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-151">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="c8e9c-152">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-152">Optional, default value is false.</span></span>|


### <a name="properties-of-an-activity-based-timeout-policy-definition"></a><span data-ttu-id="c8e9c-153">Propriedades de uma definição de política de tempo limite baseada em atividade</span><span class="sxs-lookup"><span data-stu-id="c8e9c-153">Properties of an activity-based timeout policy definition</span></span>
<span data-ttu-id="c8e9c-154">As propriedades abaixo formam o objeto JSON que representa uma política de tempo limite baseada na atividade.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-154">The properties below form the JSON object that represents an activity-based timeout policy.</span></span> <span data-ttu-id="c8e9c-155">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="c8e9c-155">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="c8e9c-156">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="c8e9c-156">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```json
{
  "definition":["{\"ActivityBasedTimeoutPolicy\":{\"Version\":1,\"ApplicationPolicies\":[{\"ApplicationId\":\"default\",\"WebSessionIdleTimeout\":\"01:00:00\"},{\"ApplicationId\":\"c44b4083-3bb0-49c1-b47d-974e53cbdf3c\",\"WebSessionIdleTimeout\":\"00:15:00\"}]}}"]
}
```

><span data-ttu-id="c8e9c-157">Observação: todas as durações de tempo nessas propriedades são especificadas no formato "dd. hh: mm: SS".</span><span class="sxs-lookup"><span data-stu-id="c8e9c-157">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="c8e9c-158">Observação: os valores máximos para propriedades denotadas em "dias" são 1 segundo curto do número de dias indicado.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-158">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="c8e9c-159">Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="c8e9c-159">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="c8e9c-160">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8e9c-160">Property</span></span>     | <span data-ttu-id="c8e9c-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8e9c-161">Type</span></span>   |<span data-ttu-id="c8e9c-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8e9c-162">Description</span></span>|
|:-------------|:------|:---------|
|<span data-ttu-id="c8e9c-163">Versão</span><span class="sxs-lookup"><span data-stu-id="c8e9c-163">Version</span></span>|<span data-ttu-id="c8e9c-164">Inteiro</span><span class="sxs-lookup"><span data-stu-id="c8e9c-164">Integer</span></span>|<span data-ttu-id="c8e9c-165">Versão da política.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-165">Policy version.</span></span> <span data-ttu-id="c8e9c-166">Defina o valor 1.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-166">Set value of 1.</span></span> <span data-ttu-id="c8e9c-167">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-167">Required.</span></span>|
|<span data-ttu-id="c8e9c-168">ApplicationPolicies</span><span class="sxs-lookup"><span data-stu-id="c8e9c-168">ApplicationPolicies</span></span>|<span data-ttu-id="c8e9c-169">Objeto JSON</span><span class="sxs-lookup"><span data-stu-id="c8e9c-169">JSON object</span></span>|<span data-ttu-id="c8e9c-170">Conjunto de políticas de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-170">Collection of application policy.</span></span> <span data-ttu-id="c8e9c-171">Uma política de aplicativo, é uma combinação de uma ApplicationId e uma WebSessionIdleTimeout:</span><span class="sxs-lookup"><span data-stu-id="c8e9c-171">An application policy, is a combination of an ApplicationId and a WebSessionIdleTimeout:</span></span> <br> <ul><li><span data-ttu-id="c8e9c-172">**ApplicationId**: valores permitidos:</span><span class="sxs-lookup"><span data-stu-id="c8e9c-172">**ApplicationId**: Allowed values:</span></span><ul><li> <span data-ttu-id="c8e9c-173">padrão: aplica a política a todos os aplicativos que dão suporte à funcionalidade de tempo limite baseada na atividade, mas não têm substituição específica do aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8e9c-173">default: applies the policy to all applications that support activity-based timeout functionality but do not have application-specific override</span></span></li><li> <span data-ttu-id="c8e9c-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c: aplica a política ao portal do Azure</span><span class="sxs-lookup"><span data-stu-id="c8e9c-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c: applies the policy to the Azure Portal</span></span></li></ul></li><li><span data-ttu-id="c8e9c-175">**WebSessionIdleTimeout**: o período de inatividade do usuário após o qual a sessão da Web do usuário é considerada expirada.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-175">**WebSessionIdleTimeout**: The period of user inactivity after which the user's web session is considered expired.</span></span> <span data-ttu-id="c8e9c-176">O valor mínimo é de 5 minutos; o valor máximo é 1 dia.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-176">The minimum value is 5 minutes; the maximum value is 1 day.</span></span></li></ul> |


## <a name="relationships"></a><span data-ttu-id="c8e9c-177">Relações</span><span class="sxs-lookup"><span data-stu-id="c8e9c-177">Relationships</span></span>

<span data-ttu-id="c8e9c-178">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8e9c-178">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8e9c-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8e9c-179">JSON representation</span></span>

<span data-ttu-id="c8e9c-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8e9c-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
  "baseType": "",
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