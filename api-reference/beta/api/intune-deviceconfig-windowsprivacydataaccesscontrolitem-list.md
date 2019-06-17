---
title: Listar windowsPrivacyDataAccessControlItems
description: Listar Propriedades e relações dos objetos windowsPrivacyDataAccessControlItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 178e873d39fa682cb7cdc67696c42698f0f2691f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961410"
---
# <a name="list-windowsprivacydataaccesscontrolitems"></a><span data-ttu-id="c0add-103">Listar windowsPrivacyDataAccessControlItems</span><span class="sxs-lookup"><span data-stu-id="c0add-103">List windowsPrivacyDataAccessControlItems</span></span>

> <span data-ttu-id="c0add-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0add-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0add-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0add-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0add-106">Listar Propriedades e relações dos objetos [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="c0add-106">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0add-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0add-107">Prerequisites</span></span>
<span data-ttu-id="c0add-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0add-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0add-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0add-110">Permission type</span></span>|<span data-ttu-id="c0add-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c0add-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0add-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0add-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0add-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0add-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c0add-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0add-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0add-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0add-115">Not supported.</span></span>|
|<span data-ttu-id="c0add-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0add-116">Application</span></span>|<span data-ttu-id="c0add-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0add-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0add-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0add-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="c0add-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0add-119">Request headers</span></span>
|<span data-ttu-id="c0add-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0add-120">Header</span></span>|<span data-ttu-id="c0add-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c0add-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0add-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0add-122">Authorization</span></span>|<span data-ttu-id="c0add-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0add-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0add-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0add-124">Accept</span></span>|<span data-ttu-id="c0add-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0add-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0add-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0add-126">Request body</span></span>
<span data-ttu-id="c0add-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0add-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0add-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0add-128">Response</span></span>
<span data-ttu-id="c0add-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0add-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0add-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0add-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0add-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0add-131">Request</span></span>
<span data-ttu-id="c0add-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0add-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

### <a name="response"></a><span data-ttu-id="c0add-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0add-133">Response</span></span>
<span data-ttu-id="c0add-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0add-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
      "id": "03b15556-5556-03b1-5655-b1035655b103",
      "accessLevel": "forceAllow",
      "dataCategory": "accountInfo",
      "appPackageFamilyName": "App Package Family Name value",
      "appDisplayName": "App Display Name value"
    }
  ]
}
```





