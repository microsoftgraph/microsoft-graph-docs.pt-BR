---
title: Tipo de recurso activityBasedTimeoutPolicy
description: Representa uma política que pode controlar o tempo de tempo ocioso para sessões da Web para aplicativos que suportam a funcionalidade de tempo-de-tempo baseado em atividade.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3d2031af6b744bbd81e4e6849e5ed78978396e8c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448881"
---
# <a name="activitybasedtimeoutpolicy-resource-type"></a><span data-ttu-id="d4272-103">Tipo de recurso activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d4272-103">activityBasedTimeoutPolicy resource type</span></span>

<span data-ttu-id="d4272-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4272-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4272-105">Representa uma política que pode controlar o tempo de tempo ocioso para sessões da Web para aplicativos que suportam a funcionalidade de tempo-de-tempo baseado em atividade.</span><span class="sxs-lookup"><span data-stu-id="d4272-105">Represents a policy that can control the idle timeout for web sessions for applications that support activity-based timeout functionality.</span></span> <span data-ttu-id="d4272-106">Os aplicativos impõem a inscrição automática após um período de inatividade.</span><span class="sxs-lookup"><span data-stu-id="d4272-106">Applications enforce automatic signout after a period of inactivity.</span></span> <span data-ttu-id="d4272-107">Esse tipo de política só pode ser aplicado no nível da organização (definindo a **propriedade isOrganizationDefault** como `true` ).</span><span class="sxs-lookup"><span data-stu-id="d4272-107">This type of policy can only be applied at the organization level (by setting the **isOrganizationDefault** property to `true`).</span></span>

<span data-ttu-id="d4272-108">Herda de [stsPolicy](stsPolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d4272-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d4272-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="d4272-109">Methods</span></span>

| <span data-ttu-id="d4272-110">Método</span><span class="sxs-lookup"><span data-stu-id="d4272-110">Method</span></span>       | <span data-ttu-id="d4272-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d4272-111">Return Type</span></span> | <span data-ttu-id="d4272-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4272-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d4272-113">Listar activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="d4272-113">List activityBasedTimeoutPolicies</span></span>](../api/activitybasedtimeoutpolicy-list.md) | [<span data-ttu-id="d4272-114">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d4272-114">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="d4272-115">Ler propriedades e relações de objetos activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="d4272-115">Read properties and relationships of activityBasedTimeoutPolicy objects.</span></span> |
| [<span data-ttu-id="d4272-116">Criar activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d4272-116">Create activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-post-activitybasedtimeoutpolicies.md) | [<span data-ttu-id="d4272-117">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d4272-117">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="d4272-118">Crie um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="d4272-118">Create an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="d4272-119">Obter activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d4272-119">Get activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-get.md) | [<span data-ttu-id="d4272-120">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d4272-120">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="d4272-121">Ler propriedades e relações de um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="d4272-121">Read properties and relationships of an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="d4272-122">Atualizar activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d4272-122">Update activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-update.md) | <span data-ttu-id="d4272-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4272-123">None</span></span> | <span data-ttu-id="d4272-124">Atualizar um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="d4272-124">Update an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="d4272-125">Excluir activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="d4272-125">Delete activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-delete.md) | <span data-ttu-id="d4272-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4272-126">None</span></span> | <span data-ttu-id="d4272-127">Exclua um objeto activityBasedTimeoutPolicy.</span><span class="sxs-lookup"><span data-stu-id="d4272-127">Delete an activityBasedTimeoutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d4272-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4272-128">Properties</span></span>

| <span data-ttu-id="d4272-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4272-129">Property</span></span>     | <span data-ttu-id="d4272-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4272-130">Type</span></span>        | <span data-ttu-id="d4272-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4272-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4272-132">id</span><span class="sxs-lookup"><span data-stu-id="d4272-132">id</span></span>|<span data-ttu-id="d4272-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4272-133">String</span></span>| <span data-ttu-id="d4272-134">Identificador exclusivo dessa política.</span><span class="sxs-lookup"><span data-stu-id="d4272-134">Unique identifier for this policy.</span></span> <span data-ttu-id="d4272-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4272-135">Read-only.</span></span>|
|<span data-ttu-id="d4272-136">definition</span><span class="sxs-lookup"><span data-stu-id="d4272-136">definition</span></span>|<span data-ttu-id="d4272-137">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4272-137">String collection</span></span>| <span data-ttu-id="d4272-138">Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política.</span><span class="sxs-lookup"><span data-stu-id="d4272-138">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="d4272-139">Consulte abaixo para obter mais detalhes sobre o esquema JSON para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="d4272-139">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="d4272-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4272-140">Required.</span></span>|
|<span data-ttu-id="d4272-141">description</span><span class="sxs-lookup"><span data-stu-id="d4272-141">description</span></span>|<span data-ttu-id="d4272-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4272-142">String</span></span>| <span data-ttu-id="d4272-143">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="d4272-143">Description for this policy.</span></span>|
|<span data-ttu-id="d4272-144">displayName</span><span class="sxs-lookup"><span data-stu-id="d4272-144">displayName</span></span>|<span data-ttu-id="d4272-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4272-145">String</span></span>| <span data-ttu-id="d4272-146">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="d4272-146">Display name for this policy.</span></span> <span data-ttu-id="d4272-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4272-147">Required.</span></span>|
|<span data-ttu-id="d4272-148">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="d4272-148">isOrganizationDefault</span></span>|<span data-ttu-id="d4272-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4272-149">Boolean</span></span>|<span data-ttu-id="d4272-150">Se definido como true, ativa essa política.</span><span class="sxs-lookup"><span data-stu-id="d4272-150">If set to true, activates this policy.</span></span> <span data-ttu-id="d4272-151">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="d4272-151">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="d4272-152">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="d4272-152">Optional, default value is false.</span></span>|


### <a name="properties-of-an-activity-based-timeout-policy-definition"></a><span data-ttu-id="d4272-153">Propriedades de uma definição de política de tempo de tempo livre baseada em atividade</span><span class="sxs-lookup"><span data-stu-id="d4272-153">Properties of an activity-based timeout policy definition</span></span>
<span data-ttu-id="d4272-154">As propriedades abaixo formam o objeto JSON que representa uma política de tempo-de-tempo baseado em atividade.</span><span class="sxs-lookup"><span data-stu-id="d4272-154">The properties below form the JSON object that represents an activity-based timeout policy.</span></span> <span data-ttu-id="d4272-155">Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com** aspas que escapam para serem inseridas na propriedade **definition.**</span><span class="sxs-lookup"><span data-stu-id="d4272-155">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="d4272-156">Um exemplo é mostrado abaixo no formato JSON:</span><span class="sxs-lookup"><span data-stu-id="d4272-156">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```json
{
  "definition":["{\"ActivityBasedTimeoutPolicy\":{\"Version\":1,\"ApplicationPolicies\":[{\"ApplicationId\":\"default\",\"WebSessionIdleTimeout\":\"01:00:00\"},{\"ApplicationId\":\"c44b4083-3bb0-49c1-b47d-974e53cbdf3c\",\"WebSessionIdleTimeout\":\"00:15:00\"}]}}"]
}
```

><span data-ttu-id="d4272-157">**Observação:** Todas as durações de tempo nessas propriedades são especificadas no formato "dd.hh:mm:ss".</span><span class="sxs-lookup"><span data-stu-id="d4272-157">**Note:** All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="d4272-158">**Observação:** Os valores máximos para propriedades anotadas em "dias" são 1 segundo a menos do número de dias anotado.</span><span class="sxs-lookup"><span data-stu-id="d4272-158">**Note:** Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="d4272-159">Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".</span><span class="sxs-lookup"><span data-stu-id="d4272-159">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="d4272-160">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4272-160">Property</span></span>     | <span data-ttu-id="d4272-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4272-161">Type</span></span>   |<span data-ttu-id="d4272-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4272-162">Description</span></span>|
|:-------------|:------|:---------|
|<span data-ttu-id="d4272-163">Versão</span><span class="sxs-lookup"><span data-stu-id="d4272-163">Version</span></span>|<span data-ttu-id="d4272-164">Inteiro</span><span class="sxs-lookup"><span data-stu-id="d4272-164">Integer</span></span>|<span data-ttu-id="d4272-165">Versão da política.</span><span class="sxs-lookup"><span data-stu-id="d4272-165">Policy version.</span></span> <span data-ttu-id="d4272-166">Definir o valor de 1.</span><span class="sxs-lookup"><span data-stu-id="d4272-166">Set value of 1.</span></span> <span data-ttu-id="d4272-167">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4272-167">Required.</span></span>|
|<span data-ttu-id="d4272-168">ApplicationPolicies</span><span class="sxs-lookup"><span data-stu-id="d4272-168">ApplicationPolicies</span></span>|<span data-ttu-id="d4272-169">Objeto JSON</span><span class="sxs-lookup"><span data-stu-id="d4272-169">JSON object</span></span>|<span data-ttu-id="d4272-170">Coleção de política de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d4272-170">Collection of application policy.</span></span> <span data-ttu-id="d4272-171">Uma política de aplicativo é uma combinação de um ApplicationId e um WebSessionIdleTimeout:</span><span class="sxs-lookup"><span data-stu-id="d4272-171">An application policy, is a combination of an ApplicationId and a WebSessionIdleTimeout:</span></span> <br> <ul><li><span data-ttu-id="d4272-172">**ApplicationId**: Valores permitidos:</span><span class="sxs-lookup"><span data-stu-id="d4272-172">**ApplicationId**: Allowed values:</span></span><ul><li> <span data-ttu-id="d4272-173">default: aplica a política a todos os aplicativos que suportam a funcionalidade de tempo-de-tempo baseado em atividade, mas não têm substituição específica do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4272-173">default: applies the policy to all applications that support activity-based timeout functionality but do not have application-specific override</span></span></li><li> <span data-ttu-id="d4272-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c: aplica a política ao Portal do Azure</span><span class="sxs-lookup"><span data-stu-id="d4272-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c: applies the policy to the Azure Portal</span></span></li></ul></li><li><span data-ttu-id="d4272-175">**WebSessionIdleTimeout**: o período de inatividade do usuário após o qual a sessão da Web do usuário é considerada expirada.</span><span class="sxs-lookup"><span data-stu-id="d4272-175">**WebSessionIdleTimeout**: The period of user inactivity after which the user's web session is considered expired.</span></span> <span data-ttu-id="d4272-176">O valor mínimo é 5 minutos; o valor máximo é 1 dia.</span><span class="sxs-lookup"><span data-stu-id="d4272-176">The minimum value is 5 minutes; the maximum value is 1 day.</span></span></li></ul> |


## <a name="relationships"></a><span data-ttu-id="d4272-177">Relações</span><span class="sxs-lookup"><span data-stu-id="d4272-177">Relationships</span></span>

<span data-ttu-id="d4272-178">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4272-178">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4272-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4272-179">JSON representation</span></span>

<span data-ttu-id="d4272-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4272-180">The following is a JSON representation of the resource.</span></span>

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

