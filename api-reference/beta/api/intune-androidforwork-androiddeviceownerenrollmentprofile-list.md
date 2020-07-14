---
title: Listar androidDeviceOwnerEnrollmentProfiles
description: Listar Propriedades e relações dos objetos androidDeviceOwnerEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4b4e3fde99b4254a7667b45473e77ff042a7a4c2
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123614"
---
# <a name="list-androiddeviceownerenrollmentprofiles"></a><span data-ttu-id="b934f-103">Listar androidDeviceOwnerEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="b934f-103">List androidDeviceOwnerEnrollmentProfiles</span></span>

<span data-ttu-id="b934f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b934f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b934f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b934f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b934f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b934f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b934f-107">Listar Propriedades e relações dos objetos [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b934f-107">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b934f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b934f-108">Prerequisites</span></span>
<span data-ttu-id="b934f-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b934f-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b934f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b934f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b934f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b934f-111">Permission type</span></span>|<span data-ttu-id="b934f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b934f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b934f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b934f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b934f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b934f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b934f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b934f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b934f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b934f-116">Not supported.</span></span>|
|<span data-ttu-id="b934f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b934f-117">Application</span></span>|<span data-ttu-id="b934f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b934f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b934f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b934f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="b934f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b934f-120">Request headers</span></span>
|<span data-ttu-id="b934f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b934f-121">Header</span></span>|<span data-ttu-id="b934f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b934f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b934f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b934f-123">Authorization</span></span>|<span data-ttu-id="b934f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b934f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b934f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b934f-125">Accept</span></span>|<span data-ttu-id="b934f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b934f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b934f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b934f-127">Request body</span></span>
<span data-ttu-id="b934f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b934f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b934f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b934f-129">Response</span></span>
<span data-ttu-id="b934f-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b934f-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b934f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b934f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b934f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b934f-132">Request</span></span>
<span data-ttu-id="b934f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b934f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="b934f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b934f-134">Response</span></span>
<span data-ttu-id="b934f-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b934f-135">Here is an example of the response.</span></span> <span data-ttu-id="b934f-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b934f-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b934f-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b934f-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 967

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
      "accountId": "Account Id value",
      "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
      "displayName": "Display Name value",
      "description": "Description value",
      "enrollmentMode": "corporateOwnedFullyManaged",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "tokenValue": "Token Value value",
      "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
      "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
      "enrolledDeviceCount": 3,
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```



