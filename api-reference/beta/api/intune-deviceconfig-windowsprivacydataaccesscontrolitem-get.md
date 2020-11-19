---
title: Obter windowsPrivacyDataAccessControlItem
description: Leia as propriedades e as relações do objeto windowsPrivacyDataAccessControlItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ce8e321baa7f70bb51a75097fa5c9ffeb76bb4ca
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49278594"
---
# <a name="get-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="4675d-103">Obter windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="4675d-103">Get windowsPrivacyDataAccessControlItem</span></span>

<span data-ttu-id="4675d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4675d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4675d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4675d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4675d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4675d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4675d-107">Leia as propriedades e as relações do objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="4675d-107">Read properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4675d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4675d-108">Prerequisites</span></span>
<span data-ttu-id="4675d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4675d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4675d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4675d-111">Permission type</span></span>|<span data-ttu-id="4675d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4675d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4675d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4675d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4675d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4675d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4675d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4675d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4675d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4675d-116">Not supported.</span></span>|
|<span data-ttu-id="4675d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4675d-117">Application</span></span>|<span data-ttu-id="4675d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4675d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4675d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4675d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4675d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4675d-120">Optional query parameters</span></span>
<span data-ttu-id="4675d-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4675d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4675d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4675d-122">Request headers</span></span>
|<span data-ttu-id="4675d-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4675d-123">Header</span></span>|<span data-ttu-id="4675d-124">Valor</span><span class="sxs-lookup"><span data-stu-id="4675d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4675d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4675d-125">Authorization</span></span>|<span data-ttu-id="4675d-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4675d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4675d-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4675d-127">Accept</span></span>|<span data-ttu-id="4675d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4675d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4675d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4675d-129">Request body</span></span>
<span data-ttu-id="4675d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4675d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4675d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4675d-131">Response</span></span>
<span data-ttu-id="4675d-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4675d-132">If successful, this method returns a `200 OK` response code and [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4675d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4675d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4675d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4675d-134">Request</span></span>
<span data-ttu-id="4675d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4675d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

### <a name="response"></a><span data-ttu-id="4675d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4675d-136">Response</span></span>
<span data-ttu-id="4675d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4675d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
    "id": "03b15556-5556-03b1-5655-b1035655b103",
    "accessLevel": "forceAllow",
    "dataCategory": "accountInfo",
    "appPackageFamilyName": "App Package Family Name value",
    "appDisplayName": "App Display Name value"
  }
}
```




