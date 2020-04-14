---
title: Atualizar onPremisesConditionalAccessSettings
description: Atualizar as propriedades de um objeto onPremisesConditionalAccessSettings.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 381b43c1b9f1f9dfc00b8711432efb4f2d8ec7c9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43377687"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="b4260-103">Atualizar onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="b4260-103">Update onPremisesConditionalAccessSettings</span></span>

<span data-ttu-id="b4260-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4260-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4260-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b4260-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4260-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4260-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4260-107">Atualizar as propriedades de um objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="b4260-107">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4260-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4260-108">Prerequisites</span></span>
<span data-ttu-id="b4260-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4260-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4260-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4260-111">Permission type</span></span>|<span data-ttu-id="b4260-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4260-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4260-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4260-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4260-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4260-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b4260-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4260-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4260-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4260-116">Not supported.</span></span>|
|<span data-ttu-id="b4260-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4260-117">Application</span></span>|<span data-ttu-id="b4260-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4260-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4260-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4260-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
PATCH /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="b4260-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4260-120">Request headers</span></span>
|<span data-ttu-id="b4260-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4260-121">Header</span></span>|<span data-ttu-id="b4260-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b4260-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4260-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4260-123">Authorization</span></span>|<span data-ttu-id="b4260-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4260-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4260-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b4260-125">Accept</span></span>|<span data-ttu-id="b4260-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4260-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4260-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4260-127">Request body</span></span>
<span data-ttu-id="b4260-128">No corpo da solicitação, forneça uma representação JSON do objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="b4260-128">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="b4260-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="b4260-129">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="b4260-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4260-130">Property</span></span>|<span data-ttu-id="b4260-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4260-131">Type</span></span>|<span data-ttu-id="b4260-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4260-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4260-133">id</span><span class="sxs-lookup"><span data-stu-id="b4260-133">id</span></span>|<span data-ttu-id="b4260-134">String</span><span class="sxs-lookup"><span data-stu-id="b4260-134">String</span></span>|<span data-ttu-id="b4260-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b4260-135">Not yet documented</span></span>|
|<span data-ttu-id="b4260-136">enabled</span><span class="sxs-lookup"><span data-stu-id="b4260-136">enabled</span></span>|<span data-ttu-id="b4260-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4260-137">Boolean</span></span>|<span data-ttu-id="b4260-138">Indica se o acesso condicional local está habilitado para esta organização</span><span class="sxs-lookup"><span data-stu-id="b4260-138">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="b4260-139">includedGroups</span><span class="sxs-lookup"><span data-stu-id="b4260-139">includedGroups</span></span>|<span data-ttu-id="b4260-140">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="b4260-140">Guid collection</span></span>|<span data-ttu-id="b4260-141">Grupos de usuários que serão direcionados pelo acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="b4260-141">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="b4260-142">Todos os usuários nesses grupos deverão ter dispositivos móveis gerenciados e compatíveis com o acesso a email.</span><span class="sxs-lookup"><span data-stu-id="b4260-142">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="b4260-143">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="b4260-143">excludedGroups</span></span>|<span data-ttu-id="b4260-144">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="b4260-144">Guid collection</span></span>|<span data-ttu-id="b4260-145">Grupos de usuários que estarão isentos ao acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="b4260-145">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="b4260-146">Todos os usuários desses grupos ficarão isentos da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="b4260-146">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="b4260-147">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="b4260-147">overrideDefaultRule</span></span>|<span data-ttu-id="b4260-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="b4260-148">Boolean</span></span>|<span data-ttu-id="b4260-149">Substitui as regras de acesso padrão ao permitir a um dispositivo que seja concedida a garantia de acesso.</span><span class="sxs-lookup"><span data-stu-id="b4260-149">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="b4260-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4260-150">Response</span></span>
<span data-ttu-id="b4260-151">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4260-151">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4260-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4260-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4260-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4260-153">Request</span></span>
<span data-ttu-id="b4260-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4260-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a><span data-ttu-id="b4260-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4260-155">Response</span></span>
<span data-ttu-id="b4260-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4260-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```



