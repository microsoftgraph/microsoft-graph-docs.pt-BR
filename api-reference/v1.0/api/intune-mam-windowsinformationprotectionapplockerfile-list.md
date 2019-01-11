---
title: Listar windowsInformationProtectionAppLockerFiles
description: Listar propriedades e relações de objetos de windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 37595c8ba1f64fa55204a5a614c140af7bf44e7e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885294"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="c8eac-103">Listar windowsInformationProtectionAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="c8eac-103">List windowsInformationProtectionAppLockerFiles</span></span>

> <span data-ttu-id="c8eac-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c8eac-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8eac-105">Listar propriedades e relações de objetos de [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="c8eac-105">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8eac-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8eac-106">Prerequisites</span></span>
<span data-ttu-id="c8eac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8eac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8eac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8eac-109">Permission type</span></span>|<span data-ttu-id="c8eac-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c8eac-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8eac-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8eac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c8eac-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8eac-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c8eac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8eac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8eac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8eac-114">Not supported.</span></span>|
|<span data-ttu-id="c8eac-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8eac-115">Application</span></span>|<span data-ttu-id="c8eac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8eac-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8eac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8eac-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c8eac-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8eac-118">Request headers</span></span>
|<span data-ttu-id="c8eac-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8eac-119">Header</span></span>|<span data-ttu-id="c8eac-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c8eac-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8eac-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8eac-121">Authorization</span></span>|<span data-ttu-id="c8eac-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8eac-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8eac-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8eac-123">Accept</span></span>|<span data-ttu-id="c8eac-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c8eac-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8eac-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8eac-125">Request body</span></span>
<span data-ttu-id="c8eac-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8eac-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8eac-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8eac-127">Response</span></span>
<span data-ttu-id="c8eac-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8eac-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8eac-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8eac-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8eac-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8eac-130">Request</span></span>
<span data-ttu-id="c8eac-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8eac-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="c8eac-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8eac-132">Response</span></span>
<span data-ttu-id="c8eac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8eac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



