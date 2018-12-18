---
title: Listar windowsInformationProtectionAppLockerFiles
description: Listar propriedades e relações de objetos de windowsInformationProtectionAppLockerFile.
author: tfitzmac
ms.openlocfilehash: d0c33fc5b529e4ab1028e811f6f0024c5ea8f63b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309552"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="05300-103">Listar windowsInformationProtectionAppLockerFiles</span><span class="sxs-lookup"><span data-stu-id="05300-103">List windowsInformationProtectionAppLockerFiles</span></span>

> <span data-ttu-id="05300-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="05300-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05300-105">Listar propriedades e relações de objetos de [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="05300-105">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05300-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05300-106">Prerequisites</span></span>
<span data-ttu-id="05300-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05300-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05300-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05300-109">Permission type</span></span>|<span data-ttu-id="05300-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05300-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05300-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05300-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05300-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="05300-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="05300-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05300-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05300-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05300-114">Not supported.</span></span>|
|<span data-ttu-id="05300-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05300-115">Application</span></span>|<span data-ttu-id="05300-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05300-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05300-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05300-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="05300-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05300-118">Request headers</span></span>
|<span data-ttu-id="05300-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05300-119">Header</span></span>|<span data-ttu-id="05300-120">Valor</span><span class="sxs-lookup"><span data-stu-id="05300-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05300-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="05300-121">Authorization</span></span>|<span data-ttu-id="05300-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05300-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05300-123">Accept</span><span class="sxs-lookup"><span data-stu-id="05300-123">Accept</span></span>|<span data-ttu-id="05300-124">application/json</span><span class="sxs-lookup"><span data-stu-id="05300-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05300-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05300-125">Request body</span></span>
<span data-ttu-id="05300-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="05300-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05300-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="05300-127">Response</span></span>
<span data-ttu-id="05300-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05300-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05300-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05300-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="05300-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05300-130">Request</span></span>
<span data-ttu-id="05300-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05300-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="05300-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="05300-132">Response</span></span>
<span data-ttu-id="05300-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05300-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



