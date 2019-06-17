---
title: Listar androidForWorkEnrollmentProfiles
description: Listar propriedades e relações dos objetos androidForWorkEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a7f46508216bb4e0ce7041f1c7b11e0defc2310f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34966520"
---
# <a name="list-androidforworkenrollmentprofiles"></a><span data-ttu-id="a4f06-103">Listar androidForWorkEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="a4f06-103">List androidForWorkEnrollmentProfiles</span></span>

> <span data-ttu-id="a4f06-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a4f06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4f06-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a4f06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4f06-106">Listar propriedades e relações dos objetos [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="a4f06-106">List properties and relationships of the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4f06-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a4f06-107">Prerequisites</span></span>
<span data-ttu-id="a4f06-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4f06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4f06-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4f06-110">Permission type</span></span>|<span data-ttu-id="a4f06-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a4f06-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4f06-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4f06-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4f06-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4f06-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a4f06-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4f06-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4f06-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4f06-115">Not supported.</span></span>|
|<span data-ttu-id="a4f06-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4f06-116">Application</span></span>|<span data-ttu-id="a4f06-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4f06-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4f06-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4f06-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="a4f06-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4f06-119">Request headers</span></span>
|<span data-ttu-id="a4f06-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a4f06-120">Header</span></span>|<span data-ttu-id="a4f06-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a4f06-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4f06-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4f06-122">Authorization</span></span>|<span data-ttu-id="a4f06-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4f06-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4f06-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a4f06-124">Accept</span></span>|<span data-ttu-id="a4f06-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4f06-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4f06-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4f06-126">Request body</span></span>
<span data-ttu-id="a4f06-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a4f06-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4f06-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4f06-128">Response</span></span>
<span data-ttu-id="a4f06-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4f06-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4f06-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4f06-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4f06-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4f06-131">Request</span></span>
<span data-ttu-id="a4f06-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4f06-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="a4f06-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4f06-133">Response</span></span>
<span data-ttu-id="a4f06-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a4f06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





