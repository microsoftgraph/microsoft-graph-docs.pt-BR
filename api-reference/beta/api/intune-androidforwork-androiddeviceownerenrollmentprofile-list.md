---
title: Listar androidDeviceOwnerEnrollmentProfiles
description: Listar propriedades e relações dos objetos androidDeviceOwnerEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc7cea90db361a567588eee305ddfe03835e0e84
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144799"
---
# <a name="list-androiddeviceownerenrollmentprofiles"></a><span data-ttu-id="a677a-103">Listar androidDeviceOwnerEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="a677a-103">List androidDeviceOwnerEnrollmentProfiles</span></span>

<span data-ttu-id="a677a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a677a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a677a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a677a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a677a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a677a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a677a-107">Listar propriedades e relações dos objetos [androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a677a-107">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a677a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a677a-108">Prerequisites</span></span>
<span data-ttu-id="a677a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a677a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a677a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a677a-111">Permission type</span></span>|<span data-ttu-id="a677a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a677a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a677a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a677a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a677a-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a677a-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a677a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a677a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a677a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a677a-116">Not supported.</span></span>|
|<span data-ttu-id="a677a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a677a-117">Application</span></span>|<span data-ttu-id="a677a-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a677a-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a677a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a677a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="a677a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a677a-120">Request headers</span></span>
|<span data-ttu-id="a677a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a677a-121">Header</span></span>|<span data-ttu-id="a677a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a677a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a677a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a677a-123">Authorization</span></span>|<span data-ttu-id="a677a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a677a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a677a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a677a-125">Accept</span></span>|<span data-ttu-id="a677a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a677a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a677a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a677a-127">Request body</span></span>
<span data-ttu-id="a677a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a677a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a677a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a677a-129">Response</span></span>
<span data-ttu-id="a677a-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a677a-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a677a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a677a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a677a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a677a-132">Request</span></span>
<span data-ttu-id="a677a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a677a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="a677a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a677a-134">Response</span></span>
<span data-ttu-id="a677a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a677a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1051

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
      "accountId": "Account Id value",
      "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
      "displayName": "Display Name value",
      "description": "Description value",
      "enrollmentMode": "corporateOwnedFullyManaged",
      "enrollmentTokenType": "corporateOwnedDedicatedDeviceWithAzureADSharedMode",
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




