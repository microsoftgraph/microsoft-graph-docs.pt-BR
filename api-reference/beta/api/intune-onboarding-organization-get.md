---
title: Obter organização
description: Leia as propriedades e as relações do objeto organização.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cfb8429f0aba8c17f3bc940a7e020be045f905df
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43377649"
---
# <a name="get-organization"></a><span data-ttu-id="b261f-103">Obter organização</span><span class="sxs-lookup"><span data-stu-id="b261f-103">Get organization</span></span>

<span data-ttu-id="b261f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b261f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b261f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b261f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b261f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b261f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b261f-107">Leia as propriedades e as relações do objeto [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="b261f-107">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b261f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b261f-108">Prerequisites</span></span>
<span data-ttu-id="b261f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b261f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b261f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b261f-111">Permission type</span></span>|<span data-ttu-id="b261f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b261f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b261f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b261f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b261f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b261f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b261f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b261f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b261f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b261f-116">Not supported.</span></span>|
|<span data-ttu-id="b261f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b261f-117">Application</span></span>|<span data-ttu-id="b261f-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b261f-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b261f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b261f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b261f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b261f-120">Optional query parameters</span></span>
<span data-ttu-id="b261f-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b261f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b261f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b261f-122">Request headers</span></span>
|<span data-ttu-id="b261f-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b261f-123">Header</span></span>|<span data-ttu-id="b261f-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b261f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b261f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b261f-125">Authorization</span></span>|<span data-ttu-id="b261f-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b261f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b261f-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b261f-127">Accept</span></span>|<span data-ttu-id="b261f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b261f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b261f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b261f-129">Request body</span></span>
<span data-ttu-id="b261f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b261f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b261f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b261f-131">Response</span></span>
<span data-ttu-id="b261f-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [organization](../resources/intune-onboarding-organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b261f-132">If successful, this method returns a `200 OK` response code and [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b261f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b261f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b261f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b261f-134">Request</span></span>
<span data-ttu-id="b261f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b261f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/organization/{organizationId}
```

### <a name="response"></a><span data-ttu-id="b261f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b261f-136">Response</span></span>
<span data-ttu-id="b261f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b261f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



