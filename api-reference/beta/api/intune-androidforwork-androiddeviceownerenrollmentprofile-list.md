---
title: Lista androidDeviceOwnerEnrollmentProfiles
description: Lista as propriedades e os relacionamentos dos objetos androidDeviceOwnerEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 79fb004fc57444f77c3110316516cb5ecec7ba31
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883157"
---
# <a name="list-androiddeviceownerenrollmentprofiles"></a><span data-ttu-id="21287-103">Lista androidDeviceOwnerEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="21287-103">List androidDeviceOwnerEnrollmentProfiles</span></span>

> <span data-ttu-id="21287-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="21287-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21287-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="21287-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21287-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="21287-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21287-107">Lista as propriedades e os relacionamentos dos objetos [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="21287-107">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21287-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21287-108">Prerequisites</span></span>
<span data-ttu-id="21287-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21287-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21287-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21287-111">Permission type</span></span>|<span data-ttu-id="21287-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21287-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21287-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21287-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21287-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21287-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="21287-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21287-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21287-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21287-116">Not supported.</span></span>|
|<span data-ttu-id="21287-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21287-117">Application</span></span>|<span data-ttu-id="21287-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21287-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21287-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21287-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="21287-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21287-120">Request headers</span></span>
|<span data-ttu-id="21287-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21287-121">Header</span></span>|<span data-ttu-id="21287-122">Valor</span><span class="sxs-lookup"><span data-stu-id="21287-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21287-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="21287-123">Authorization</span></span>|<span data-ttu-id="21287-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21287-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21287-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21287-125">Accept</span></span>|<span data-ttu-id="21287-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21287-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21287-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21287-127">Request body</span></span>
<span data-ttu-id="21287-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21287-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21287-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="21287-129">Response</span></span>
<span data-ttu-id="21287-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21287-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21287-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21287-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="21287-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21287-132">Request</span></span>
<span data-ttu-id="21287-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21287-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="21287-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="21287-134">Response</span></span>
<span data-ttu-id="21287-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21287-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 838

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
      }
    }
  ]
}
```





