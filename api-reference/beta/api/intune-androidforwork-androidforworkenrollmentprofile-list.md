---
title: Listar androidForWorkEnrollmentProfiles
description: Listar propriedades e relações dos objetos androidForWorkEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2e380beb6587f8d9af4523ef2a51c435a56de332
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402654"
---
# <a name="list-androidforworkenrollmentprofiles"></a><span data-ttu-id="51c2e-103">Listar androidForWorkEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="51c2e-103">List androidForWorkEnrollmentProfiles</span></span>

> <span data-ttu-id="51c2e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="51c2e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="51c2e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="51c2e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51c2e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="51c2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51c2e-107">Listar propriedades e relações dos objetos [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="51c2e-107">List properties and relationships of the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51c2e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51c2e-108">Prerequisites</span></span>
<span data-ttu-id="51c2e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="51c2e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="51c2e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51c2e-111">Permission type</span></span>|<span data-ttu-id="51c2e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51c2e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51c2e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51c2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51c2e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="51c2e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="51c2e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51c2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51c2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51c2e-116">Not supported.</span></span>|
|<span data-ttu-id="51c2e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51c2e-117">Application</span></span>|<span data-ttu-id="51c2e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51c2e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51c2e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51c2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="51c2e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51c2e-120">Request headers</span></span>
|<span data-ttu-id="51c2e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51c2e-121">Header</span></span>|<span data-ttu-id="51c2e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="51c2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51c2e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="51c2e-123">Authorization</span></span>|<span data-ttu-id="51c2e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51c2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51c2e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51c2e-125">Accept</span></span>|<span data-ttu-id="51c2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51c2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51c2e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51c2e-127">Request body</span></span>
<span data-ttu-id="51c2e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51c2e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51c2e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="51c2e-129">Response</span></span>
<span data-ttu-id="51c2e-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51c2e-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51c2e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51c2e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="51c2e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51c2e-132">Request</span></span>
<span data-ttu-id="51c2e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51c2e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="51c2e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="51c2e-134">Response</span></span>
<span data-ttu-id="51c2e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51c2e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




