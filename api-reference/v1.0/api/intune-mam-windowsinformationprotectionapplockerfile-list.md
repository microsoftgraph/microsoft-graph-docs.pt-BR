---
title: Listar windowsInformationProtectionAppLockerFiles
description: Listar propriedades e relações de objetos de windowsInformationProtectionAppLockerFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6de9e213849341f64ee350c592fb3b5ccf6f1b1c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363007"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="7260b-103">Listar windowsInformationProtectionAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="7260b-103">List windowsInformationProtectionAppLockerFiles</span></span>

> <span data-ttu-id="7260b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7260b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7260b-105">Listar propriedades e relações de objetos de [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="7260b-105">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7260b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7260b-106">Prerequisites</span></span>
<span data-ttu-id="7260b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7260b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7260b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7260b-109">Permission type</span></span>|<span data-ttu-id="7260b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7260b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7260b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7260b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7260b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7260b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7260b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7260b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7260b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7260b-114">Not supported.</span></span>|
|<span data-ttu-id="7260b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7260b-115">Application</span></span>|<span data-ttu-id="7260b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7260b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7260b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7260b-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="7260b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7260b-118">Request headers</span></span>
|<span data-ttu-id="7260b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7260b-119">Header</span></span>|<span data-ttu-id="7260b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7260b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7260b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7260b-121">Authorization</span></span>|<span data-ttu-id="7260b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7260b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7260b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7260b-123">Accept</span></span>|<span data-ttu-id="7260b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7260b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7260b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7260b-125">Request body</span></span>
<span data-ttu-id="7260b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7260b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7260b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7260b-127">Response</span></span>
<span data-ttu-id="7260b-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7260b-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7260b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7260b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7260b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7260b-130">Request</span></span>
<span data-ttu-id="7260b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7260b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="7260b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7260b-132">Response</span></span>
<span data-ttu-id="7260b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7260b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




