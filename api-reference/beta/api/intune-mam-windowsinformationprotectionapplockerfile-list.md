---
title: Listar windowsInformationProtectionAppLockerFiles
description: Listar propriedades e relações de objetos de windowsInformationProtectionAppLockerFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 76392bb3ef32b0ef98852a28dafd9ebd70dbd9ee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014445"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="eb33c-103">Listar windowsInformationProtectionAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="eb33c-103">List windowsInformationProtectionAppLockerFiles</span></span>

<span data-ttu-id="eb33c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb33c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb33c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb33c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb33c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb33c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb33c-107">Listar propriedades e relações de objetos de [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="eb33c-107">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb33c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb33c-108">Prerequisites</span></span>
<span data-ttu-id="eb33c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb33c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb33c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb33c-111">Permission type</span></span>|<span data-ttu-id="eb33c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb33c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb33c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb33c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eb33c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb33c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="eb33c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb33c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb33c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb33c-116">Not supported.</span></span>|
|<span data-ttu-id="eb33c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb33c-117">Application</span></span>|<span data-ttu-id="eb33c-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb33c-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb33c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb33c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="eb33c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb33c-120">Request headers</span></span>
|<span data-ttu-id="eb33c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb33c-121">Header</span></span>|<span data-ttu-id="eb33c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eb33c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb33c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb33c-123">Authorization</span></span>|<span data-ttu-id="eb33c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb33c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb33c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb33c-125">Accept</span></span>|<span data-ttu-id="eb33c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb33c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb33c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb33c-127">Request body</span></span>
<span data-ttu-id="eb33c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb33c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb33c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb33c-129">Response</span></span>
<span data-ttu-id="eb33c-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb33c-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb33c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb33c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb33c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb33c-132">Request</span></span>
<span data-ttu-id="eb33c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb33c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="eb33c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb33c-134">Response</span></span>
<span data-ttu-id="eb33c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb33c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
      "displayName": "Display Name value",
      "fileHash": "File Hash value",
      "file": "ZmlsZQ==",
      "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
      "version": "Version value"
    }
  ]
}
```






