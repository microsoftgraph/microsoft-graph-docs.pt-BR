---
title: Listar windowsInformationProtectionAppLockerFiles
description: Listar propriedades e relações de objetos de windowsInformationProtectionAppLockerFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d4437ef303aed3486c0978fd1a9f0c19a86d6efd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512843"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="5b85f-103">Listar windowsInformationProtectionAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="5b85f-103">List windowsInformationProtectionAppLockerFiles</span></span>

<span data-ttu-id="5b85f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b85f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b85f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b85f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b85f-106">Listar propriedades e relações de objetos de [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="5b85f-106">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b85f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5b85f-107">Prerequisites</span></span>
<span data-ttu-id="5b85f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b85f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b85f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b85f-110">Permission type</span></span>|<span data-ttu-id="5b85f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5b85f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b85f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b85f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b85f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b85f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5b85f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b85f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b85f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b85f-115">Not supported.</span></span>|
|<span data-ttu-id="5b85f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b85f-116">Application</span></span>|<span data-ttu-id="5b85f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b85f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b85f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b85f-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5b85f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b85f-119">Request headers</span></span>
|<span data-ttu-id="5b85f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b85f-120">Header</span></span>|<span data-ttu-id="5b85f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5b85f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b85f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b85f-122">Authorization</span></span>|<span data-ttu-id="5b85f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b85f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b85f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5b85f-124">Accept</span></span>|<span data-ttu-id="5b85f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b85f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b85f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b85f-126">Request body</span></span>
<span data-ttu-id="5b85f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b85f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b85f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b85f-128">Response</span></span>
<span data-ttu-id="5b85f-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b85f-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b85f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b85f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b85f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b85f-131">Request</span></span>
<span data-ttu-id="5b85f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b85f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="5b85f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b85f-133">Response</span></span>
<span data-ttu-id="5b85f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b85f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




