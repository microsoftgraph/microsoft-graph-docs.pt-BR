---
title: Listar androidDeviceOwnerEnrollmentProfiles
description: Listar Propriedades e relações dos objetos androidDeviceOwnerEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74cb5100feb61e76103e448a20b88c8953a51fc6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705209"
---
# <a name="list-androiddeviceownerenrollmentprofiles"></a><span data-ttu-id="cbc3c-103">Listar androidDeviceOwnerEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="cbc3c-103">List androidDeviceOwnerEnrollmentProfiles</span></span>

> <span data-ttu-id="cbc3c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cbc3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbc3c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cbc3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbc3c-106">Listar Propriedades e relações dos objetos [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="cbc3c-106">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbc3c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cbc3c-107">Prerequisites</span></span>
<span data-ttu-id="cbc3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbc3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbc3c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbc3c-110">Permission type</span></span>|<span data-ttu-id="cbc3c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cbc3c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbc3c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbc3c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cbc3c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbc3c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cbc3c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbc3c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbc3c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbc3c-115">Not supported.</span></span>|
|<span data-ttu-id="cbc3c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbc3c-116">Application</span></span>|<span data-ttu-id="cbc3c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbc3c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbc3c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbc3c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="cbc3c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbc3c-119">Request headers</span></span>
|<span data-ttu-id="cbc3c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cbc3c-120">Header</span></span>|<span data-ttu-id="cbc3c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cbc3c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbc3c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbc3c-122">Authorization</span></span>|<span data-ttu-id="cbc3c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbc3c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbc3c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cbc3c-124">Accept</span></span>|<span data-ttu-id="cbc3c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cbc3c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbc3c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbc3c-126">Request body</span></span>
<span data-ttu-id="cbc3c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cbc3c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbc3c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbc3c-128">Response</span></span>
<span data-ttu-id="cbc3c-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbc3c-129">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbc3c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbc3c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbc3c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbc3c-131">Request</span></span>
<span data-ttu-id="cbc3c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbc3c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="cbc3c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbc3c-133">Response</span></span>
<span data-ttu-id="cbc3c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbc3c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 898

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
      "accountId": "Account Id value",
      "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
      "displayName": "Display Name value",
      "description": "Description value",
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
      "scopeTags": [
        "Scope Tags value"
      ]
    }
  ]
}
```





