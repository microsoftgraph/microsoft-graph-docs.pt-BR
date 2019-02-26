---
title: Listar targetedManagedAppConfigurations
description: Listar propriedades e relações dos objetos targetedManagedAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b5845c1b0fb1ef3b59fa679bdc0d064984408194
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263599"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="7d357-103">Listar targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="7d357-103">List targetedManagedAppConfigurations</span></span>

> <span data-ttu-id="7d357-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d357-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d357-105">Listar propriedades e relações dos objetos [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d357-105">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d357-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d357-106">Prerequisites</span></span>
<span data-ttu-id="7d357-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7d357-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7d357-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d357-109">Permission type</span></span>|<span data-ttu-id="7d357-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d357-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d357-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d357-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7d357-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d357-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7d357-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d357-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d357-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d357-114">Not supported.</span></span>|
|<span data-ttu-id="7d357-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d357-115">Application</span></span>|<span data-ttu-id="7d357-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d357-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d357-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d357-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7d357-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d357-118">Request headers</span></span>
|<span data-ttu-id="7d357-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d357-119">Header</span></span>|<span data-ttu-id="7d357-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7d357-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d357-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d357-121">Authorization</span></span>|<span data-ttu-id="7d357-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d357-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d357-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d357-123">Accept</span></span>|<span data-ttu-id="7d357-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7d357-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d357-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d357-125">Request body</span></span>
<span data-ttu-id="7d357-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d357-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d357-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d357-127">Response</span></span>
<span data-ttu-id="7d357-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d357-128">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d357-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d357-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d357-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d357-130">Request</span></span>
<span data-ttu-id="7d357-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d357-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="7d357-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d357-132">Response</span></span>
<span data-ttu-id="7d357-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d357-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



