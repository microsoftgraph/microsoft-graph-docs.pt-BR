---
title: Listar deviceEnrollmentLimitConfigurations
description: Listar propriedades e relações de objetos de deviceEnrollmentLimitConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b89e3b6fc65794d6a45fbafc410b4537ef16156
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179429"
---
# <a name="list-deviceenrollmentlimitconfigurations"></a><span data-ttu-id="3c483-103">Listar deviceEnrollmentLimitConfigurations</span><span class="sxs-lookup"><span data-stu-id="3c483-103">List deviceEnrollmentLimitConfigurations</span></span>

<span data-ttu-id="3c483-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c483-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c483-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c483-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c483-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c483-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c483-107">Listar propriedades e relações de objetos de [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3c483-107">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c483-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c483-108">Prerequisites</span></span>
<span data-ttu-id="3c483-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c483-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c483-111">Permission type</span></span>|<span data-ttu-id="3c483-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c483-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c483-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c483-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c483-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c483-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3c483-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c483-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c483-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c483-116">Not supported.</span></span>|
|<span data-ttu-id="3c483-117">Application</span><span class="sxs-lookup"><span data-stu-id="3c483-117">Application</span></span>|<span data-ttu-id="3c483-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c483-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c483-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c483-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3c483-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c483-120">Request headers</span></span>
|<span data-ttu-id="3c483-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c483-121">Header</span></span>|<span data-ttu-id="3c483-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3c483-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c483-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c483-123">Authorization</span></span>|<span data-ttu-id="3c483-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c483-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c483-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c483-125">Accept</span></span>|<span data-ttu-id="3c483-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c483-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c483-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c483-127">Request body</span></span>
<span data-ttu-id="3c483-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c483-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c483-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c483-129">Response</span></span>
<span data-ttu-id="3c483-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c483-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c483-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c483-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c483-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c483-132">Request</span></span>
<span data-ttu-id="3c483-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c483-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="3c483-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c483-134">Response</span></span>
<span data-ttu-id="3c483-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c483-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 520

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
      "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "limit": 5
    }
  ]
}
```



