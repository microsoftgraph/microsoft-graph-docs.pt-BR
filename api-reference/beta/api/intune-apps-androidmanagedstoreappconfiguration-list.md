---
title: Listar androidManagedStoreAppConfigurations
description: Listar Propriedades e relações dos objetos androidManagedStoreAppConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 239b69fa17a8f5daaf26bc5cd7caa36b3704c40d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762235"
---
# <a name="list-androidmanagedstoreappconfigurations"></a><span data-ttu-id="485d2-103">Listar androidManagedStoreAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="485d2-103">List androidManagedStoreAppConfigurations</span></span>

> <span data-ttu-id="485d2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="485d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="485d2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="485d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="485d2-106">Listar Propriedades e relações dos objetos [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="485d2-106">List properties and relationships of the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="485d2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="485d2-107">Prerequisites</span></span>
<span data-ttu-id="485d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="485d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="485d2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="485d2-110">Permission type</span></span>|<span data-ttu-id="485d2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="485d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="485d2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="485d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="485d2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="485d2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="485d2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="485d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="485d2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="485d2-115">Not supported.</span></span>|
|<span data-ttu-id="485d2-116">Application</span><span class="sxs-lookup"><span data-stu-id="485d2-116">Application</span></span>|<span data-ttu-id="485d2-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="485d2-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="485d2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="485d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="485d2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="485d2-119">Request headers</span></span>
|<span data-ttu-id="485d2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="485d2-120">Header</span></span>|<span data-ttu-id="485d2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="485d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="485d2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="485d2-122">Authorization</span></span>|<span data-ttu-id="485d2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="485d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="485d2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="485d2-124">Accept</span></span>|<span data-ttu-id="485d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="485d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="485d2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="485d2-126">Request body</span></span>
<span data-ttu-id="485d2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="485d2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="485d2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="485d2-128">Response</span></span>
<span data-ttu-id="485d2-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="485d2-129">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="485d2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="485d2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="485d2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="485d2-131">Request</span></span>
<span data-ttu-id="485d2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="485d2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="485d2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="485d2-133">Response</span></span>
<span data-ttu-id="485d2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="485d2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 889

{
  "value": [
    {
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
      "appSupportsOemConfig": true
    }
  ]
}
```




