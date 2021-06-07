---
title: Atualizar onPremisesConditionalAccessSettings
description: Atualizar as propriedades de um objeto onPremisesConditionalAccessSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7691e10a3877b9bb29bdc27e62b5d5790925513b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757972"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="02aa5-103">Atualizar onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="02aa5-103">Update onPremisesConditionalAccessSettings</span></span>

<span data-ttu-id="02aa5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02aa5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02aa5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02aa5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02aa5-106">Atualizar as propriedades de um objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="02aa5-106">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02aa5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02aa5-107">Prerequisites</span></span>
<span data-ttu-id="02aa5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02aa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02aa5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02aa5-110">Permission type</span></span>|<span data-ttu-id="02aa5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02aa5-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02aa5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02aa5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02aa5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02aa5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="02aa5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02aa5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02aa5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02aa5-115">Not supported.</span></span>|
|<span data-ttu-id="02aa5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02aa5-116">Application</span></span>|<span data-ttu-id="02aa5-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02aa5-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02aa5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02aa5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="02aa5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02aa5-119">Request headers</span></span>
|<span data-ttu-id="02aa5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02aa5-120">Header</span></span>|<span data-ttu-id="02aa5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="02aa5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02aa5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="02aa5-122">Authorization</span></span>|<span data-ttu-id="02aa5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02aa5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02aa5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02aa5-124">Accept</span></span>|<span data-ttu-id="02aa5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02aa5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02aa5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02aa5-126">Request body</span></span>
<span data-ttu-id="02aa5-127">No corpo da solicitação, forneça uma representação JSON do objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="02aa5-127">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="02aa5-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="02aa5-128">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="02aa5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02aa5-129">Property</span></span>|<span data-ttu-id="02aa5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="02aa5-130">Type</span></span>|<span data-ttu-id="02aa5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="02aa5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02aa5-132">id</span><span class="sxs-lookup"><span data-stu-id="02aa5-132">id</span></span>|<span data-ttu-id="02aa5-133">String</span><span class="sxs-lookup"><span data-stu-id="02aa5-133">String</span></span>|<span data-ttu-id="02aa5-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="02aa5-134">Not yet documented</span></span>|
|<span data-ttu-id="02aa5-135">enabled</span><span class="sxs-lookup"><span data-stu-id="02aa5-135">enabled</span></span>|<span data-ttu-id="02aa5-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="02aa5-136">Boolean</span></span>|<span data-ttu-id="02aa5-137">Indica se o acesso condicional local está habilitado para esta organização</span><span class="sxs-lookup"><span data-stu-id="02aa5-137">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="02aa5-138">includedGroups</span><span class="sxs-lookup"><span data-stu-id="02aa5-138">includedGroups</span></span>|<span data-ttu-id="02aa5-139">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="02aa5-139">Guid collection</span></span>|<span data-ttu-id="02aa5-140">Grupos de usuários que serão direcionados pelo acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="02aa5-140">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="02aa5-141">Todos os usuários nesses grupos deverão ter dispositivos móveis gerenciados e compatíveis com o acesso a email.</span><span class="sxs-lookup"><span data-stu-id="02aa5-141">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="02aa5-142">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="02aa5-142">excludedGroups</span></span>|<span data-ttu-id="02aa5-143">Coleção de GUIDs</span><span class="sxs-lookup"><span data-stu-id="02aa5-143">Guid collection</span></span>|<span data-ttu-id="02aa5-144">Grupos de usuários que estarão isentos ao acesso condicional local.</span><span class="sxs-lookup"><span data-stu-id="02aa5-144">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="02aa5-145">Todos os usuários desses grupos ficarão isentos da política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="02aa5-145">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="02aa5-146">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="02aa5-146">overrideDefaultRule</span></span>|<span data-ttu-id="02aa5-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="02aa5-147">Boolean</span></span>|<span data-ttu-id="02aa5-148">Substitui as regras de acesso padrão ao permitir a um dispositivo que seja concedida a garantia de acesso.</span><span class="sxs-lookup"><span data-stu-id="02aa5-148">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="02aa5-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="02aa5-149">Response</span></span>
<span data-ttu-id="02aa5-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02aa5-150">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02aa5-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02aa5-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="02aa5-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02aa5-152">Request</span></span>
<span data-ttu-id="02aa5-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02aa5-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="02aa5-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="02aa5-154">Response</span></span>
<span data-ttu-id="02aa5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02aa5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




