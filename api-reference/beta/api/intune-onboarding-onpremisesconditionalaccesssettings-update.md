---
title: Atualizar onPremisesConditionalAccessSettings
description: Atualizar as propriedades de um objeto onPremisesConditionalAccessSettings.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7ef2b656fcf4bca020c7f1cc9f3e74881946413
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528635"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="7fde8-103">Atualizar onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="7fde8-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="7fde8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7fde8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fde8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7fde8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fde8-106">Atualizar as propriedades de um objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="7fde8-106">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fde8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7fde8-107">Prerequisites</span></span>
<span data-ttu-id="7fde8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fde8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fde8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fde8-110">Permission type</span></span>|<span data-ttu-id="7fde8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7fde8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fde8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fde8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7fde8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fde8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7fde8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fde8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fde8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fde8-115">Not supported.</span></span>|
|<span data-ttu-id="7fde8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fde8-116">Application</span></span>|<span data-ttu-id="7fde8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fde8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fde8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fde8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
PATCH /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="7fde8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fde8-119">Request headers</span></span>
|<span data-ttu-id="7fde8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7fde8-120">Header</span></span>|<span data-ttu-id="7fde8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7fde8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fde8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fde8-122">Authorization</span></span>|<span data-ttu-id="7fde8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fde8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fde8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7fde8-124">Accept</span></span>|<span data-ttu-id="7fde8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7fde8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fde8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fde8-126">Request body</span></span>
<span data-ttu-id="7fde8-127">No corpo da solicitação, forneça uma representação JSON do objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="7fde8-127">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="7fde8-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="7fde8-128">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="7fde8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7fde8-129">Property</span></span>|<span data-ttu-id="7fde8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7fde8-130">Type</span></span>|<span data-ttu-id="7fde8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fde8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fde8-132">id</span><span class="sxs-lookup"><span data-stu-id="7fde8-132">id</span></span>|<span data-ttu-id="7fde8-133">String</span><span class="sxs-lookup"><span data-stu-id="7fde8-133">String</span></span>|<span data-ttu-id="7fde8-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7fde8-134">Not yet documented</span></span>|
|<span data-ttu-id="7fde8-135">enabled</span><span class="sxs-lookup"><span data-stu-id="7fde8-135">enabled</span></span>|<span data-ttu-id="7fde8-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fde8-136">Boolean</span></span>|<span data-ttu-id="7fde8-137">Indica se o acesso condicional local está habilitado para esta organização</span><span class="sxs-lookup"><span data-stu-id="7fde8-137">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="7fde8-138">includedGroups</span><span class="sxs-lookup"><span data-stu-id="7fde8-138">includedGroups</span></span>|<span data-ttu-id="7fde8-139">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="7fde8-139">Guid collection</span></span>|<span data-ttu-id="7fde8-140">Grupos de usuários que serão direcionados pelo acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="7fde8-140">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="7fde8-141">Todos os usuários nesses grupos deverão ter dispositivos móveis gerenciados e compatíveis com o acesso a email.</span><span class="sxs-lookup"><span data-stu-id="7fde8-141">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="7fde8-142">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="7fde8-142">excludedGroups</span></span>|<span data-ttu-id="7fde8-143">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="7fde8-143">Guid collection</span></span>|<span data-ttu-id="7fde8-144">Grupos de usuários que estarão isentos ao acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="7fde8-144">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="7fde8-145">Todos os usuários desses grupos ficarão isentos da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="7fde8-145">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="7fde8-146">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="7fde8-146">overrideDefaultRule</span></span>|<span data-ttu-id="7fde8-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="7fde8-147">Boolean</span></span>|<span data-ttu-id="7fde8-148">Substitui as regras de acesso padrão ao permitir a um dispositivo que seja concedida a garantia de acesso.</span><span class="sxs-lookup"><span data-stu-id="7fde8-148">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="7fde8-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fde8-149">Response</span></span>
<span data-ttu-id="7fde8-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fde8-150">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fde8-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fde8-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fde8-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fde8-152">Request</span></span>
<span data-ttu-id="7fde8-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fde8-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7fde8-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fde8-154">Response</span></span>
<span data-ttu-id="7fde8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fde8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





