---
title: ação importOffice365DeviceConfigurationPolicies
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 51f97db40ad94525a5db1afa803cddd2bb0694c1
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793180"
---
# <a name="importoffice365deviceconfigurationpolicies-action"></a><span data-ttu-id="21556-103">ação importOffice365DeviceConfigurationPolicies</span><span class="sxs-lookup"><span data-stu-id="21556-103">importOffice365DeviceConfigurationPolicies action</span></span>

<span data-ttu-id="21556-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21556-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21556-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21556-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21556-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21556-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21556-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="21556-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21556-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21556-108">Prerequisites</span></span>
<span data-ttu-id="21556-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21556-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21556-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21556-111">Permission type</span></span>|<span data-ttu-id="21556-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21556-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21556-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21556-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21556-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21556-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="21556-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21556-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21556-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21556-116">Not supported.</span></span>|
|<span data-ttu-id="21556-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21556-117">Application</span></span>|<span data-ttu-id="21556-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21556-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21556-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21556-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/importOffice365DeviceConfigurationPolicies
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/importOffice365DeviceConfigurationPolicies
```

## <a name="request-headers"></a><span data-ttu-id="21556-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21556-120">Request headers</span></span>
|<span data-ttu-id="21556-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21556-121">Header</span></span>|<span data-ttu-id="21556-122">Valor</span><span class="sxs-lookup"><span data-stu-id="21556-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21556-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="21556-123">Authorization</span></span>|<span data-ttu-id="21556-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21556-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21556-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21556-125">Accept</span></span>|<span data-ttu-id="21556-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21556-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21556-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21556-127">Request body</span></span>
<span data-ttu-id="21556-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21556-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21556-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="21556-129">Response</span></span>
<span data-ttu-id="21556-130">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e uma coleção [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21556-130">If successful, this action returns a `200 OK` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21556-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21556-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="21556-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21556-132">Request</span></span>
<span data-ttu-id="21556-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21556-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/importOffice365DeviceConfigurationPolicies
```

### <a name="response"></a><span data-ttu-id="21556-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="21556-134">Response</span></span>
<span data-ttu-id="21556-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21556-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 452

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntent",
      "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
      "displayName": "Display Name value",
      "description": "Description value",
      "isAssigned": true,
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "templateId": "Template Id value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```


