---
title: Obter androidDeviceOwnerEnrollmentProfile
description: Leia as propriedades e as relações do objeto androidDeviceOwnerEnrollmentProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4923e3f1de3240c15efc67e8c3741eab171a5010
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815793"
---
# <a name="get-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="e90bb-103">Obter androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e90bb-103">Get androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="e90bb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e90bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e90bb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e90bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e90bb-106">Leia as propriedades e as relações do objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e90bb-106">Read properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e90bb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e90bb-107">Prerequisites</span></span>
<span data-ttu-id="e90bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e90bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e90bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e90bb-110">Permission type</span></span>|<span data-ttu-id="e90bb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e90bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e90bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e90bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e90bb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e90bb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e90bb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e90bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e90bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e90bb-115">Not supported.</span></span>|
|<span data-ttu-id="e90bb-116">Application</span><span class="sxs-lookup"><span data-stu-id="e90bb-116">Application</span></span>|<span data-ttu-id="e90bb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e90bb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e90bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e90bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e90bb-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e90bb-119">Optional query parameters</span></span>
<span data-ttu-id="e90bb-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e90bb-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e90bb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e90bb-121">Request headers</span></span>
|<span data-ttu-id="e90bb-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e90bb-122">Header</span></span>|<span data-ttu-id="e90bb-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e90bb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e90bb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e90bb-124">Authorization</span></span>|<span data-ttu-id="e90bb-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e90bb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e90bb-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e90bb-126">Accept</span></span>|<span data-ttu-id="e90bb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e90bb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e90bb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e90bb-128">Request body</span></span>
<span data-ttu-id="e90bb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e90bb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e90bb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e90bb-130">Response</span></span>
<span data-ttu-id="e90bb-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e90bb-131">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e90bb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e90bb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e90bb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e90bb-133">Request</span></span>
<span data-ttu-id="e90bb-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e90bb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="e90bb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e90bb-135">Response</span></span>
<span data-ttu-id="e90bb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e90bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 858

{
  "value": {
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
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




