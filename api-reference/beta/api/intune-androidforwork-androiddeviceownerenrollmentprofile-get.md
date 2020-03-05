---
title: Obter androidDeviceOwnerEnrollmentProfile
description: Leia as propriedades e as relações do objeto androidDeviceOwnerEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cde03448bb92755ae839b45bcaf6860c4066eba8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446286"
---
# <a name="get-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="d39c6-103">Obter androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d39c6-103">Get androidDeviceOwnerEnrollmentProfile</span></span>

<span data-ttu-id="d39c6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d39c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d39c6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d39c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d39c6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d39c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d39c6-107">Leia as propriedades e as relações do objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d39c6-107">Read properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d39c6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d39c6-108">Prerequisites</span></span>
<span data-ttu-id="d39c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d39c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d39c6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d39c6-111">Permission type</span></span>|<span data-ttu-id="d39c6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d39c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d39c6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d39c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d39c6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d39c6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d39c6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d39c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d39c6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d39c6-116">Not supported.</span></span>|
|<span data-ttu-id="d39c6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d39c6-117">Application</span></span>|<span data-ttu-id="d39c6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d39c6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d39c6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d39c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d39c6-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d39c6-120">Optional query parameters</span></span>
<span data-ttu-id="d39c6-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d39c6-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d39c6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d39c6-122">Request headers</span></span>
|<span data-ttu-id="d39c6-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d39c6-123">Header</span></span>|<span data-ttu-id="d39c6-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d39c6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d39c6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d39c6-125">Authorization</span></span>|<span data-ttu-id="d39c6-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d39c6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d39c6-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d39c6-127">Accept</span></span>|<span data-ttu-id="d39c6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d39c6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d39c6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d39c6-129">Request body</span></span>
<span data-ttu-id="d39c6-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d39c6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d39c6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d39c6-131">Response</span></span>
<span data-ttu-id="d39c6-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d39c6-132">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d39c6-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d39c6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d39c6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d39c6-134">Request</span></span>
<span data-ttu-id="d39c6-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d39c6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="d39c6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d39c6-136">Response</span></span>
<span data-ttu-id="d39c6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d39c6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





