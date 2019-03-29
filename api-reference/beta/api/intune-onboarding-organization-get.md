---
title: Obter organização
description: Leia as propriedades e as relações do objeto organização.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c7eef2cf09e04728206cae427646e1fbc3da15a1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971119"
---
# <a name="get-organization"></a><span data-ttu-id="e83dc-103">Obter organização</span><span class="sxs-lookup"><span data-stu-id="e83dc-103">Get organization</span></span>

> <span data-ttu-id="e83dc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e83dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e83dc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e83dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e83dc-106">Leia as propriedades e as relações do objeto [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e83dc-106">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e83dc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e83dc-107">Prerequisites</span></span>
<span data-ttu-id="e83dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e83dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e83dc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e83dc-110">Permission type</span></span>|<span data-ttu-id="e83dc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e83dc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e83dc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e83dc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e83dc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e83dc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e83dc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e83dc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e83dc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e83dc-115">Not supported.</span></span>|
|<span data-ttu-id="e83dc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e83dc-116">Application</span></span>|<span data-ttu-id="e83dc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e83dc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e83dc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e83dc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e83dc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e83dc-119">Optional query parameters</span></span>
<span data-ttu-id="e83dc-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e83dc-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e83dc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e83dc-121">Request headers</span></span>
|<span data-ttu-id="e83dc-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e83dc-122">Header</span></span>|<span data-ttu-id="e83dc-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e83dc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e83dc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e83dc-124">Authorization</span></span>|<span data-ttu-id="e83dc-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e83dc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e83dc-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e83dc-126">Accept</span></span>|<span data-ttu-id="e83dc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e83dc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e83dc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e83dc-128">Request body</span></span>
<span data-ttu-id="e83dc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e83dc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e83dc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e83dc-130">Response</span></span>
<span data-ttu-id="e83dc-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [organization](../resources/intune-onboarding-organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e83dc-131">If successful, this method returns a `200 OK` response code and [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e83dc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e83dc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e83dc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e83dc-133">Request</span></span>
<span data-ttu-id="e83dc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e83dc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/organization/{organizationId}
```

### <a name="response"></a><span data-ttu-id="e83dc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e83dc-135">Response</span></span>
<span data-ttu-id="e83dc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e83dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




