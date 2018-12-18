---
title: Listar targetedManagedAppConfigurations
description: Listar propriedades e relações dos objetos targetedManagedAppConfiguration.
author: tfitzmac
ms.openlocfilehash: fc9b6bd3c2851a46ebbdb5bfe4929f8609ed5a2f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324042"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="814f6-103">Listar targetedManagedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="814f6-103">List targetedManagedAppConfigurations</span></span>

> <span data-ttu-id="814f6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="814f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="814f6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="814f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="814f6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="814f6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="814f6-107">Listar propriedades e relações dos objetos [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="814f6-107">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="814f6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="814f6-108">Prerequisites</span></span>
<span data-ttu-id="814f6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="814f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="814f6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="814f6-111">Permission type</span></span>|<span data-ttu-id="814f6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="814f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="814f6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="814f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="814f6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="814f6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="814f6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="814f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="814f6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="814f6-116">Not supported.</span></span>|
|<span data-ttu-id="814f6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="814f6-117">Application</span></span>|<span data-ttu-id="814f6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="814f6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="814f6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="814f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="814f6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="814f6-120">Request headers</span></span>
|<span data-ttu-id="814f6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="814f6-121">Header</span></span>|<span data-ttu-id="814f6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="814f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="814f6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="814f6-123">Authorization</span></span>|<span data-ttu-id="814f6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="814f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="814f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="814f6-125">Accept</span></span>|<span data-ttu-id="814f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="814f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="814f6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="814f6-127">Request body</span></span>
<span data-ttu-id="814f6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="814f6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="814f6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="814f6-129">Response</span></span>
<span data-ttu-id="814f6-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="814f6-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="814f6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="814f6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="814f6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="814f6-132">Request</span></span>
<span data-ttu-id="814f6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="814f6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="814f6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="814f6-134">Response</span></span>
<span data-ttu-id="814f6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="814f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





