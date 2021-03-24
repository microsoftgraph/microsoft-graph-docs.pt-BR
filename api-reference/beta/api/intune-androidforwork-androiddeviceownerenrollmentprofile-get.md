---
title: Obter androidDeviceOwnerEnrollmentProfile
description: Leia propriedades e relações do objeto androidDeviceOwnerEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b1997a59dec589121cfd25ce9f0412eba0096dee
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141369"
---
# <a name="get-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="1bd91-103">Obter androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="1bd91-103">Get androidDeviceOwnerEnrollmentProfile</span></span>

<span data-ttu-id="1bd91-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bd91-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bd91-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1bd91-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bd91-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1bd91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bd91-107">Leia propriedades e relações do [objeto androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1bd91-107">Read properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bd91-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1bd91-108">Prerequisites</span></span>
<span data-ttu-id="1bd91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bd91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bd91-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bd91-111">Permission type</span></span>|<span data-ttu-id="1bd91-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1bd91-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bd91-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bd91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1bd91-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bd91-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1bd91-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bd91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bd91-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bd91-116">Not supported.</span></span>|
|<span data-ttu-id="1bd91-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bd91-117">Application</span></span>|<span data-ttu-id="1bd91-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bd91-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bd91-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bd91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1bd91-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1bd91-120">Optional query parameters</span></span>
<span data-ttu-id="1bd91-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1bd91-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1bd91-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bd91-122">Request headers</span></span>
|<span data-ttu-id="1bd91-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1bd91-123">Header</span></span>|<span data-ttu-id="1bd91-124">Valor</span><span class="sxs-lookup"><span data-stu-id="1bd91-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bd91-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bd91-125">Authorization</span></span>|<span data-ttu-id="1bd91-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bd91-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bd91-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1bd91-127">Accept</span></span>|<span data-ttu-id="1bd91-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1bd91-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bd91-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bd91-129">Request body</span></span>
<span data-ttu-id="1bd91-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1bd91-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bd91-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bd91-131">Response</span></span>
<span data-ttu-id="1bd91-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bd91-132">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bd91-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bd91-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bd91-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bd91-134">Request</span></span>
<span data-ttu-id="1bd91-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bd91-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="1bd91-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bd91-136">Response</span></span>
<span data-ttu-id="1bd91-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bd91-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 993

{
  "value": {
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
}
```




