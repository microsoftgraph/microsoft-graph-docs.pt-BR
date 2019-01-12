---
title: Lista androidManagedStoreAppConfigurations
description: Lista as propriedades e os relacionamentos dos objetos androidManagedStoreAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 538de6c0c5a8e5ee65c78838ddb7a22b6ab5d645
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914651"
---
# <a name="list-androidmanagedstoreappconfigurations"></a><span data-ttu-id="7972c-103">Lista androidManagedStoreAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="7972c-103">List androidManagedStoreAppConfigurations</span></span>

> <span data-ttu-id="7972c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7972c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7972c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7972c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7972c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7972c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7972c-107">Lista as propriedades e os relacionamentos dos objetos [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7972c-107">List properties and relationships of the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7972c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7972c-108">Prerequisites</span></span>
<span data-ttu-id="7972c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7972c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7972c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7972c-111">Permission type</span></span>|<span data-ttu-id="7972c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7972c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7972c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7972c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7972c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7972c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7972c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7972c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7972c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7972c-116">Not supported.</span></span>|
|<span data-ttu-id="7972c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7972c-117">Application</span></span>|<span data-ttu-id="7972c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7972c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7972c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7972c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7972c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7972c-120">Request headers</span></span>
|<span data-ttu-id="7972c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7972c-121">Header</span></span>|<span data-ttu-id="7972c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7972c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7972c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7972c-123">Authorization</span></span>|<span data-ttu-id="7972c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7972c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7972c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7972c-125">Accept</span></span>|<span data-ttu-id="7972c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7972c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7972c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7972c-127">Request body</span></span>
<span data-ttu-id="7972c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7972c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7972c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7972c-129">Response</span></span>
<span data-ttu-id="7972c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7972c-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7972c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7972c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7972c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7972c-132">Request</span></span>
<span data-ttu-id="7972c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7972c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="7972c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7972c-134">Response</span></span>
<span data-ttu-id="7972c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7972c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 852

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
      ]
    }
  ]
}
```





