---
title: Atualizar onPremisesConditionalAccessSettings
description: Atualizar as propriedades de um objeto onPremisesConditionalAccessSettings.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1e77767900b40fc3f921d9d3ffd34fd6930bf19c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024081"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="8171a-103">Atualizar onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="8171a-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="8171a-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8171a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8171a-105">Atualizar as propriedades de um objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="8171a-105">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8171a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8171a-106">Prerequisites</span></span>
<span data-ttu-id="8171a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8171a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8171a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8171a-109">Permission type</span></span>|<span data-ttu-id="8171a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8171a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8171a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8171a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8171a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8171a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8171a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8171a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8171a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8171a-114">Not supported.</span></span>|
|<span data-ttu-id="8171a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8171a-115">Application</span></span>|<span data-ttu-id="8171a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8171a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8171a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8171a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="8171a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8171a-118">Request headers</span></span>
|<span data-ttu-id="8171a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8171a-119">Header</span></span>|<span data-ttu-id="8171a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8171a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8171a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8171a-121">Authorization</span></span>|<span data-ttu-id="8171a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8171a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8171a-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8171a-123">Accept</span></span>|<span data-ttu-id="8171a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8171a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8171a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8171a-125">Request body</span></span>
<span data-ttu-id="8171a-126">No corpo da solicitação, forneça uma representação JSON do objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="8171a-126">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="8171a-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="8171a-127">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="8171a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8171a-128">Property</span></span>|<span data-ttu-id="8171a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8171a-129">Type</span></span>|<span data-ttu-id="8171a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8171a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8171a-131">id</span><span class="sxs-lookup"><span data-stu-id="8171a-131">id</span></span>|<span data-ttu-id="8171a-132">String</span><span class="sxs-lookup"><span data-stu-id="8171a-132">String</span></span>|<span data-ttu-id="8171a-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8171a-133">Not yet documented</span></span>|
|<span data-ttu-id="8171a-134">enabled</span><span class="sxs-lookup"><span data-stu-id="8171a-134">enabled</span></span>|<span data-ttu-id="8171a-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="8171a-135">Boolean</span></span>|<span data-ttu-id="8171a-136">Indica se o acesso condicional local está habilitado para esta organização</span><span class="sxs-lookup"><span data-stu-id="8171a-136">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="8171a-137">includedGroups</span><span class="sxs-lookup"><span data-stu-id="8171a-137">includedGroups</span></span>|<span data-ttu-id="8171a-138">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="8171a-138">Guid collection</span></span>|<span data-ttu-id="8171a-139">Grupos de usuários que serão direcionados pelo acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="8171a-139">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="8171a-140">Todos os usuários nesses grupos deverão ter dispositivos móveis gerenciados e compatíveis com o acesso a email.</span><span class="sxs-lookup"><span data-stu-id="8171a-140">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="8171a-141">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="8171a-141">excludedGroups</span></span>|<span data-ttu-id="8171a-142">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="8171a-142">Guid collection</span></span>|<span data-ttu-id="8171a-143">Grupos de usuários que estarão isentos ao acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="8171a-143">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="8171a-144">Todos os usuários desses grupos ficarão isentos da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="8171a-144">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="8171a-145">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="8171a-145">overrideDefaultRule</span></span>|<span data-ttu-id="8171a-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="8171a-146">Boolean</span></span>|<span data-ttu-id="8171a-147">Substitui as regras de acesso padrão ao permitir a um dispositivo que seja concedida a garantia de acesso.</span><span class="sxs-lookup"><span data-stu-id="8171a-147">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="8171a-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="8171a-148">Response</span></span>
<span data-ttu-id="8171a-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8171a-149">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8171a-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8171a-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="8171a-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8171a-151">Request</span></span>
<span data-ttu-id="8171a-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8171a-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
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

### <a name="response"></a><span data-ttu-id="8171a-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="8171a-153">Response</span></span>
<span data-ttu-id="8171a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8171a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



