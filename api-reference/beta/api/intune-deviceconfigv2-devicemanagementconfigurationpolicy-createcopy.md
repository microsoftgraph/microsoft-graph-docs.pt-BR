---
title: Ação createCopy
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 353c55305eb0a09cdf26beecf1cf5e222338af3b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868356"
---
# <a name="createcopy-action"></a><span data-ttu-id="e6835-103">Ação createCopy</span><span class="sxs-lookup"><span data-stu-id="e6835-103">createCopy action</span></span>

<span data-ttu-id="e6835-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6835-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6835-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6835-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6835-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6835-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6835-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e6835-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6835-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6835-108">Prerequisites</span></span>
<span data-ttu-id="e6835-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6835-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6835-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6835-111">Permission type</span></span>|<span data-ttu-id="e6835-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6835-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6835-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6835-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6835-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6835-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6835-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6835-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6835-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6835-116">Not supported.</span></span>|
|<span data-ttu-id="e6835-117">Application</span><span class="sxs-lookup"><span data-stu-id="e6835-117">Application</span></span>|<span data-ttu-id="e6835-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6835-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6835-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6835-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/createCopy
POST /deviceManagement/reusablePolicySettings/{deviceManagementReusablePolicySettingId}/referencingConfigurationPolicies/{deviceManagementConfigurationPolicyId}/createCopy
```

## <a name="request-headers"></a><span data-ttu-id="e6835-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6835-120">Request headers</span></span>
|<span data-ttu-id="e6835-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6835-121">Header</span></span>|<span data-ttu-id="e6835-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e6835-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6835-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6835-123">Authorization</span></span>|<span data-ttu-id="e6835-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6835-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6835-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e6835-125">Accept</span></span>|<span data-ttu-id="e6835-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6835-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6835-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6835-127">Request body</span></span>
<span data-ttu-id="e6835-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e6835-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e6835-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="e6835-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e6835-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6835-130">Property</span></span>|<span data-ttu-id="e6835-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6835-131">Type</span></span>|<span data-ttu-id="e6835-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6835-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6835-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e6835-133">displayName</span></span>|<span data-ttu-id="e6835-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6835-134">String</span></span>|<span data-ttu-id="e6835-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e6835-135">Not yet documented</span></span>|
|<span data-ttu-id="e6835-136">description</span><span class="sxs-lookup"><span data-stu-id="e6835-136">description</span></span>|<span data-ttu-id="e6835-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6835-137">String</span></span>|<span data-ttu-id="e6835-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e6835-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e6835-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6835-139">Response</span></span>
<span data-ttu-id="e6835-140">Se tiver êxito, essa ação retornará um código de `200 OK` resposta e um [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6835-140">If successful, this action returns a `200 OK` response code and a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6835-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6835-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6835-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6835-142">Request</span></span>
<span data-ttu-id="e6835-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6835-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/createCopy

Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="e6835-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6835-144">Response</span></span>
<span data-ttu-id="e6835-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6835-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
    "id": "3ffd7cd0-7cd0-3ffd-d07c-fd3fd07cfd3f",
    "name": "Name value",
    "description": "Description value",
    "platforms": "macOS",
    "technologies": "mdm",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "settingCount": 12,
    "creationSource": "Creation Source value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "isAssigned": true,
    "templateReference": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
      "templateId": "Template Id value",
      "templateFamily": "endpointSecurityAntivirus",
      "templateDisplayName": "Template Display Name value",
      "templateDisplayVersion": "Template Display Version value"
    }
  }
}
```




