---
title: Listar targetedManagedAppConfigurations
description: Listar propriedades e relações dos objetos targetedManagedAppConfiguration.
author: tfitzmac
ms.openlocfilehash: 088c210d9c6df3ff403bd68e92a98b522528e3c1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343901"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="8143d-103">Listar targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="8143d-103">List targetedManagedAppConfigurations</span></span>

> <span data-ttu-id="8143d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8143d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8143d-105">Listar propriedades e relações dos objetos [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8143d-105">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8143d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8143d-106">Prerequisites</span></span>
<span data-ttu-id="8143d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8143d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8143d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8143d-109">Permission type</span></span>|<span data-ttu-id="8143d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8143d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8143d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8143d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8143d-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8143d-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8143d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8143d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8143d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8143d-114">Not supported.</span></span>|
|<span data-ttu-id="8143d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8143d-115">Application</span></span>|<span data-ttu-id="8143d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8143d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8143d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8143d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8143d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8143d-118">Request headers</span></span>
|<span data-ttu-id="8143d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8143d-119">Header</span></span>|<span data-ttu-id="8143d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8143d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8143d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8143d-121">Authorization</span></span>|<span data-ttu-id="8143d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8143d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8143d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8143d-123">Accept</span></span>|<span data-ttu-id="8143d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8143d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8143d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8143d-125">Request body</span></span>
<span data-ttu-id="8143d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8143d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8143d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8143d-127">Response</span></span>
<span data-ttu-id="8143d-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8143d-128">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8143d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8143d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8143d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8143d-130">Request</span></span>
<span data-ttu-id="8143d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8143d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="8143d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8143d-132">Response</span></span>
<span data-ttu-id="8143d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8143d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 657

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "2444e029-e029-2444-29e0-442429e04424",
      "version": "Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "deployedAppCount": 0,
      "isAssigned": true
    }
  ]
}
```



