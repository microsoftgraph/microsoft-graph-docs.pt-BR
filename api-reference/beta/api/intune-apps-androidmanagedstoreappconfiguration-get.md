---
title: Obter androidManagedStoreAppConfiguration
description: Leia as propriedades e as relações do objeto androidManagedStoreAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 61e64db548da2463d3daf6d90554374fe12cd3e2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49253584"
---
# <a name="get-androidmanagedstoreappconfiguration"></a><span data-ttu-id="c4161-103">Obter androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c4161-103">Get androidManagedStoreAppConfiguration</span></span>

<span data-ttu-id="c4161-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4161-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4161-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4161-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4161-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4161-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4161-107">Leia as propriedades e as relações do objeto [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c4161-107">Read properties and relationships of the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4161-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4161-108">Prerequisites</span></span>
<span data-ttu-id="c4161-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4161-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4161-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4161-111">Permission type</span></span>|<span data-ttu-id="c4161-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4161-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4161-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4161-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4161-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4161-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c4161-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4161-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4161-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4161-116">Not supported.</span></span>|
|<span data-ttu-id="c4161-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4161-117">Application</span></span>|<span data-ttu-id="c4161-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4161-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4161-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4161-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4161-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c4161-120">Optional query parameters</span></span>
<span data-ttu-id="c4161-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c4161-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4161-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4161-122">Request headers</span></span>
|<span data-ttu-id="c4161-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4161-123">Header</span></span>|<span data-ttu-id="c4161-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c4161-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4161-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4161-125">Authorization</span></span>|<span data-ttu-id="c4161-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4161-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4161-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4161-127">Accept</span></span>|<span data-ttu-id="c4161-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c4161-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4161-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4161-129">Request body</span></span>
<span data-ttu-id="c4161-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4161-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4161-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4161-131">Response</span></span>
<span data-ttu-id="c4161-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4161-132">If successful, this method returns a `200 OK` response code and [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4161-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4161-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4161-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4161-134">Request</span></span>
<span data-ttu-id="c4161-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4161-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c4161-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4161-136">Response</span></span>
<span data-ttu-id="c4161-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4161-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 880

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
    "id": "919a9335-9335-919a-3593-9a9135939a91",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "packageId": "Package Id value",
    "payloadJson": "Payload Json value",
    "permissionActions": [
      {
        "@odata.type": "microsoft.graph.androidPermissionAction",
        "permission": "Permission value",
        "action": "autoGrant"
      }
    ],
    "appSupportsOemConfig": true,
    "profileApplicability": "androidWorkProfile"
  }
}
```




