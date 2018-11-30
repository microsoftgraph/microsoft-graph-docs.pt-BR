---
title: Obter organização
description: Leia as propriedades e as relações do objeto organização.
ms.openlocfilehash: ffb2001973d1e0b34beef72df09a9a2e9ff3755e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034999"
---
# <a name="get-organization"></a><span data-ttu-id="cece2-103">Obter organização</span><span class="sxs-lookup"><span data-stu-id="cece2-103">Get organization</span></span>

> <span data-ttu-id="cece2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cece2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cece2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cece2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cece2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cece2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cece2-107">Leia as propriedades e as relações do objeto [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="cece2-107">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cece2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cece2-108">Prerequisites</span></span>
<span data-ttu-id="cece2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cece2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cece2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cece2-111">Permission type</span></span>|<span data-ttu-id="cece2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cece2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cece2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cece2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cece2-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cece2-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="cece2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cece2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cece2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cece2-116">Not supported.</span></span>|
|<span data-ttu-id="cece2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cece2-117">Application</span></span>|<span data-ttu-id="cece2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cece2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cece2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cece2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cece2-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cece2-120">Optional query parameters</span></span>
<span data-ttu-id="cece2-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cece2-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cece2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cece2-122">Request headers</span></span>
|<span data-ttu-id="cece2-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cece2-123">Header</span></span>|<span data-ttu-id="cece2-124">Valor</span><span class="sxs-lookup"><span data-stu-id="cece2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cece2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="cece2-125">Authorization</span></span>|<span data-ttu-id="cece2-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cece2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cece2-127">Accept</span><span class="sxs-lookup"><span data-stu-id="cece2-127">Accept</span></span>|<span data-ttu-id="cece2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cece2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cece2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cece2-129">Request body</span></span>
<span data-ttu-id="cece2-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cece2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cece2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="cece2-131">Response</span></span>
<span data-ttu-id="cece2-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [organization](../resources/intune-onboarding-organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cece2-132">If successful, this method returns a `200 OK` response code and [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cece2-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cece2-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="cece2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cece2-134">Request</span></span>
<span data-ttu-id="cece2-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cece2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/organization/{organizationId}
```

### <a name="response"></a><span data-ttu-id="cece2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cece2-136">Response</span></span>
<span data-ttu-id="cece2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cece2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 584

{
  "value": {
    "@odata.type": "#microsoft.graph.organization",
    "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
    "mobileDeviceManagementAuthority": "intune",
    "certificateConnectorSetting": {
      "@odata.type": "microsoft.graph.certificateConnectorSetting",
      "status": 6,
      "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
      "enrollmentError": "Enrollment Error value",
      "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
      "connectorVersion": "Connector Version value",
      "lastUploadVersion": 1
    }
  }
}
```





