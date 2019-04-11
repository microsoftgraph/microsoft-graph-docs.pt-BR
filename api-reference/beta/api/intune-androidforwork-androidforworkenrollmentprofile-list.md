---
title: Listar androidForWorkEnrollmentProfiles
description: Listar propriedades e relações dos objetos androidForWorkEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43b657a9e3512b8dec4fa6bce0ad92dfb3165f6c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803483"
---
# <a name="list-androidforworkenrollmentprofiles"></a><span data-ttu-id="900be-103">Listar androidForWorkEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="900be-103">List androidForWorkEnrollmentProfiles</span></span>

> <span data-ttu-id="900be-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="900be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="900be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="900be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="900be-106">Listar propriedades e relações dos objetos [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="900be-106">List properties and relationships of the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="900be-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="900be-107">Prerequisites</span></span>
<span data-ttu-id="900be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="900be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="900be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="900be-110">Permission type</span></span>|<span data-ttu-id="900be-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="900be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="900be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="900be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="900be-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="900be-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="900be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="900be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="900be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="900be-115">Not supported.</span></span>|
|<span data-ttu-id="900be-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="900be-116">Application</span></span>|<span data-ttu-id="900be-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="900be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="900be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="900be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="900be-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="900be-119">Request headers</span></span>
|<span data-ttu-id="900be-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="900be-120">Header</span></span>|<span data-ttu-id="900be-121">Valor</span><span class="sxs-lookup"><span data-stu-id="900be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="900be-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="900be-122">Authorization</span></span>|<span data-ttu-id="900be-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="900be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="900be-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="900be-124">Accept</span></span>|<span data-ttu-id="900be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="900be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="900be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="900be-126">Request body</span></span>
<span data-ttu-id="900be-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="900be-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="900be-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="900be-128">Response</span></span>
<span data-ttu-id="900be-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="900be-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="900be-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="900be-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="900be-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="900be-131">Request</span></span>
<span data-ttu-id="900be-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="900be-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="900be-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="900be-133">Response</span></span>
<span data-ttu-id="900be-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="900be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 765

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
      "accountId": "Account Id value",
      "id": "e6742553-2553-e674-5325-74e6532574e6",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "tokenValue": "Token Value value",
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





