---
title: Obter windowsPrivacyDataAccessControlItem
description: Leia as propriedades e os relacionamentos do objeto windowsPrivacyDataAccessControlItem.
ms.openlocfilehash: e349240a82bdd292b7f94c25a57475b2fdcce468
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034491"
---
# <a name="get-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="9956e-103">Obter windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="9956e-103">Get windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="9956e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9956e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9956e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9956e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9956e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9956e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9956e-107">Leia as propriedades e os relacionamentos do objeto [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="9956e-107">Read properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9956e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9956e-108">Prerequisites</span></span>
<span data-ttu-id="9956e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9956e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9956e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9956e-111">Permission type</span></span>|<span data-ttu-id="9956e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9956e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9956e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9956e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9956e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9956e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9956e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9956e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9956e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9956e-116">Not supported.</span></span>|
|<span data-ttu-id="9956e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9956e-117">Application</span></span>|<span data-ttu-id="9956e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9956e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9956e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9956e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9956e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9956e-120">Optional query parameters</span></span>
<span data-ttu-id="9956e-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9956e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9956e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9956e-122">Request headers</span></span>
|<span data-ttu-id="9956e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9956e-123">Header</span></span>|<span data-ttu-id="9956e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="9956e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9956e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9956e-125">Authorization</span></span>|<span data-ttu-id="9956e-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9956e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9956e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9956e-127">Accept</span></span>|<span data-ttu-id="9956e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9956e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9956e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9956e-129">Request body</span></span>
<span data-ttu-id="9956e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9956e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9956e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9956e-131">Response</span></span>
<span data-ttu-id="9956e-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9956e-132">If successful, this method returns a `200 OK` response code and [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9956e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9956e-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="9956e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9956e-134">Request</span></span>
<span data-ttu-id="9956e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9956e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

### <a name="response"></a><span data-ttu-id="9956e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9956e-136">Response</span></span>
<span data-ttu-id="9956e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9956e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





