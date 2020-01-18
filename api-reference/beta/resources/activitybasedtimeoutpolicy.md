---
title: tipo de recurso activityBasedTimeoutPolicy
description: Representa uma política que pode controlar o tempo limite de ociosidade para sessões da Web para aplicativos que dão suporte à funcionalidade de tempo limite baseada na atividade.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 63cadf11e2368d28d861236ec028d48a079b7840
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234129"
---
# <a name="activitybasedtimeoutpolicy-resource-type"></a><span data-ttu-id="d2865-103">tipo de recurso activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d2865-103">activityBasedTimeoutPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2865-104">Representa uma política que pode controlar o tempo limite de ociosidade para sessões da Web para aplicativos que dão suporte à funcionalidade de tempo limite baseada na atividade.</span><span class="sxs-lookup"><span data-stu-id="d2865-104">Represents a policy that can control the idle timeout for web sessions for applications that support activity-based timeout functionality.</span></span> <span data-ttu-id="d2865-105">Os aplicativos impõem a desconexão automática após um período de inatividade.</span><span class="sxs-lookup"><span data-stu-id="d2865-105">Applications enforce automatic signout after a period of inactivity.</span></span> <span data-ttu-id="d2865-106">Esse tipo de política só pode ser aplicado no nível da organização (Configurando \*\*\*\* a propriedade isOrganizationDefault `true`para).</span><span class="sxs-lookup"><span data-stu-id="d2865-106">This type of policy can only be applied at the organization level (by setting the **isOrganizationDefault** property to `true`).</span></span>

<span data-ttu-id="d2865-107">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d2865-107">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d2865-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d2865-108">Methods</span></span>

| <span data-ttu-id="d2865-109">Método</span><span class="sxs-lookup"><span data-stu-id="d2865-109">Method</span></span>       | <span data-ttu-id="d2865-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d2865-110">Return Type</span></span> | <span data-ttu-id="d2865-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2865-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d2865-112">Criar activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d2865-112">Create activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-post-activitybasedtimeoutpolicies.md) | [<span data-ttu-id="d2865-113">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d2865-113">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="d2865-114">Criar um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="d2865-114">Create an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="d2865-115">Obter activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d2865-115">Get activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-get.md) | [<span data-ttu-id="d2865-116">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d2865-116">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="d2865-117">Ler propriedades e relações de um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="d2865-117">Read properties and relationships of an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="d2865-118">Listar activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="d2865-118">List activityBasedTimeoutPolicies</span></span>](../api/activitybasedtimeoutpolicy-list.md) | [<span data-ttu-id="d2865-119">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d2865-119">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="d2865-120">Ler propriedades e relações de objetos activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="d2865-120">Read properties and relationships of activityBasedTimeoutPolicy objects.</span></span> |
| [<span data-ttu-id="d2865-121">Atualizar activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d2865-121">Update activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-update.md) | <span data-ttu-id="d2865-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d2865-122">None</span></span> | <span data-ttu-id="d2865-123">Atualize um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="d2865-123">Update an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="d2865-124">Excluir activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d2865-124">Delete activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-delete.md) | <span data-ttu-id="d2865-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d2865-125">None</span></span> | <span data-ttu-id="d2865-126">Excluir um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="d2865-126">Delete an activityBasedTimeoutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d2865-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2865-127">Properties</span></span>

| <span data-ttu-id="d2865-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2865-128">Property</span></span>     | <span data-ttu-id="d2865-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2865-129">Type</span></span>        | <span data-ttu-id="d2865-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2865-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d2865-131">id</span><span class="sxs-lookup"><span data-stu-id="d2865-131">id</span></span>|<span data-ttu-id="d2865-132">String</span><span class="sxs-lookup"><span data-stu-id="d2865-132">String</span></span>| <span data-ttu-id="d2865-133">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="d2865-133">Unique identifier for this policy.</span></span> <span data-ttu-id="d2865-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d2865-134">Read-only.</span></span>|
|<span data-ttu-id="d2865-135">definir</span><span class="sxs-lookup"><span data-stu-id="d2865-135">definition</span></span>|<span data-ttu-id="d2865-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2865-136">String collection</span></span>| <span data-ttu-id="d2865-137">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="d2865-137">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="d2865-138">Veja mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="d2865-138">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="d2865-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2865-139">Required.</span></span>|
|<span data-ttu-id="d2865-140">description</span><span class="sxs-lookup"><span data-stu-id="d2865-140">description</span></span>|<span data-ttu-id="d2865-141">String</span><span class="sxs-lookup"><span data-stu-id="d2865-141">String</span></span>| <span data-ttu-id="d2865-142">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="d2865-142">Description for this policy.</span></span>|
|<span data-ttu-id="d2865-143">displayName</span><span class="sxs-lookup"><span data-stu-id="d2865-143">displayName</span></span>|<span data-ttu-id="d2865-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2865-144">String</span></span>| <span data-ttu-id="d2865-145">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="d2865-145">Display name for this policy.</span></span> <span data-ttu-id="d2865-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2865-146">Required.</span></span>|
|<span data-ttu-id="d2865-147">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="d2865-147">isOrganizationDefault</span></span>|<span data-ttu-id="d2865-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="d2865-148">Boolean</span></span>|<span data-ttu-id="d2865-149">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="d2865-149">If set to true, activates this policy.</span></span> <span data-ttu-id="d2865-150">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="d2865-150">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="d2865-151">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="d2865-151">Optional, default value is false.</span></span>|


### <a name="properties-of-an-activity-based-timeout-policy-definition"></a><span data-ttu-id="d2865-152">Propriedades de uma definição de política de tempo limite baseada em atividade</span><span class="sxs-lookup"><span data-stu-id="d2865-152">Properties of an activity-based timeout policy definition</span></span>
<span data-ttu-id="d2865-153">As propriedades abaixo formam o objeto JSON que representa uma política de tempo limite baseada na atividade.</span><span class="sxs-lookup"><span data-stu-id="d2865-153">The properties below form the JSON object that represents an activity-based timeout policy.</span></span> <span data-ttu-id="d2865-154">Este objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade **Definition** .</span><span class="sxs-lookup"><span data-stu-id="d2865-154">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="d2865-155">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="d2865-155">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```json
{
  "definition":["{\"ActivityBasedTimeoutPolicy\":{\"Version\":1,\"ApplicationPolicies\":[{\"ApplicationId\":\"default\",\"WebSessionIdleTimeout\":\"01:00:00\"},{\"ApplicationId\":\"c44b4083-3bb0-49c1-b47d-974e53cbdf3c\",\"WebSessionIdleTimeout\":\"00:15:00\"}]}}"]
}
```

><span data-ttu-id="d2865-156">Observação: todas as durações de tempo nessas propriedades são especificadas no formato "dd. hh: mm: SS".</span><span class="sxs-lookup"><span data-stu-id="d2865-156">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="d2865-157">Observação: os valores máximos para propriedades denotadas em "dias" são 1 segundo curto do número de dias indicado.</span><span class="sxs-lookup"><span data-stu-id="d2865-157">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="d2865-158">Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="d2865-158">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="d2865-159">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2865-159">Property</span></span>     | <span data-ttu-id="d2865-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2865-160">Type</span></span>   |<span data-ttu-id="d2865-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2865-161">Description</span></span>|
|:-------------|:------|:---------|
|<span data-ttu-id="d2865-162">Versão</span><span class="sxs-lookup"><span data-stu-id="d2865-162">Version</span></span>|<span data-ttu-id="d2865-163">Inteiro</span><span class="sxs-lookup"><span data-stu-id="d2865-163">Integer</span></span>|<span data-ttu-id="d2865-164">Versão da política.</span><span class="sxs-lookup"><span data-stu-id="d2865-164">Policy version.</span></span> <span data-ttu-id="d2865-165">Defina o valor 1.</span><span class="sxs-lookup"><span data-stu-id="d2865-165">Set value of 1.</span></span> <span data-ttu-id="d2865-166">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2865-166">Required.</span></span>|
|<span data-ttu-id="d2865-167">ApplicationPolicies</span><span class="sxs-lookup"><span data-stu-id="d2865-167">ApplicationPolicies</span></span>|<span data-ttu-id="d2865-168">Objeto JSON</span><span class="sxs-lookup"><span data-stu-id="d2865-168">JSON object</span></span>|<span data-ttu-id="d2865-169">Conjunto de políticas de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d2865-169">Collection of application policy.</span></span> <span data-ttu-id="d2865-170">Uma política de aplicativo, é uma combinação de uma ApplicationId e uma WebSessionIdleTimeout:</span><span class="sxs-lookup"><span data-stu-id="d2865-170">An application policy, is a combination of an ApplicationId and a WebSessionIdleTimeout:</span></span> <br> <ul><li><span data-ttu-id="d2865-171">**ApplicationId**: valores permitidos:</span><span class="sxs-lookup"><span data-stu-id="d2865-171">**ApplicationId**: Allowed values:</span></span><ul><li> <span data-ttu-id="d2865-172">padrão: aplica a política a todos os aplicativos que dão suporte à funcionalidade de tempo limite baseada na atividade, mas não têm substituição específica do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2865-172">default: applies the policy to all applications that support activity-based timeout functionality but do not have application-specific override</span></span></li><li> <span data-ttu-id="d2865-173">c44b4083-3bb0-49c1-b47d-974e53cbdf3c: aplica a política ao portal do Azure</span><span class="sxs-lookup"><span data-stu-id="d2865-173">c44b4083-3bb0-49c1-b47d-974e53cbdf3c: applies the policy to the Azure Portal</span></span></li></ul></li><li><span data-ttu-id="d2865-174">**WebSessionIdleTimeout**: o período de inatividade do usuário após o qual a sessão da Web do usuário é considerada expirada.</span><span class="sxs-lookup"><span data-stu-id="d2865-174">**WebSessionIdleTimeout**: The period of user inactivity after which the user's web session is considered expired.</span></span> <span data-ttu-id="d2865-175">O valor mínimo é de 5 minutos; o valor máximo é 1 dia.</span><span class="sxs-lookup"><span data-stu-id="d2865-175">The minimum value is 5 minutes; the maximum value is 1 day.</span></span></li></ul> |


## <a name="relationships"></a><span data-ttu-id="d2865-176">Relações</span><span class="sxs-lookup"><span data-stu-id="d2865-176">Relationships</span></span>

<span data-ttu-id="d2865-177">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2865-177">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2865-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2865-178">JSON representation</span></span>

<span data-ttu-id="d2865-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2865-179">The following is a JSON representation of the resource.</span></span>

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