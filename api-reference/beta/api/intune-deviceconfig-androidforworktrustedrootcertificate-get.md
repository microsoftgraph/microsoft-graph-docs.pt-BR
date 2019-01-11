---
title: Obter androidForWorkTrustedRootCertificate
description: Leia as propriedades e os relacionamentos do objeto androidForWorkTrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4462604921c8b90545beb863e98b5abc40526f49
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820647"
---
# <a name="get-androidforworktrustedrootcertificate"></a><span data-ttu-id="06033-103">Obter androidForWorkTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="06033-103">Get androidForWorkTrustedRootCertificate</span></span>

> <span data-ttu-id="06033-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="06033-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06033-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="06033-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06033-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="06033-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06033-107">Leia as propriedades e os relacionamentos do objeto [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="06033-107">Read properties and relationships of the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06033-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06033-108">Prerequisites</span></span>
<span data-ttu-id="06033-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06033-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06033-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06033-111">Permission type</span></span>|<span data-ttu-id="06033-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06033-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06033-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06033-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06033-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="06033-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="06033-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06033-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06033-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06033-116">Not supported.</span></span>|
|<span data-ttu-id="06033-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06033-117">Application</span></span>|<span data-ttu-id="06033-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06033-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06033-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06033-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06033-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="06033-120">Optional query parameters</span></span>
<span data-ttu-id="06033-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="06033-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="06033-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06033-122">Request headers</span></span>
|<span data-ttu-id="06033-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06033-123">Header</span></span>|<span data-ttu-id="06033-124">Valor</span><span class="sxs-lookup"><span data-stu-id="06033-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06033-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="06033-125">Authorization</span></span>|<span data-ttu-id="06033-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06033-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06033-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06033-127">Accept</span></span>|<span data-ttu-id="06033-128">application/json</span><span class="sxs-lookup"><span data-stu-id="06033-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06033-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06033-129">Request body</span></span>
<span data-ttu-id="06033-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06033-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06033-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="06033-131">Response</span></span>
<span data-ttu-id="06033-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06033-132">If successful, this method returns a `200 OK` response code and [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06033-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06033-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="06033-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06033-134">Request</span></span>
<span data-ttu-id="06033-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06033-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
```

### <a name="response"></a><span data-ttu-id="06033-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="06033-136">Response</span></span>
<span data-ttu-id="06033-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06033-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 591

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
    "id": "2f78834c-834c-2f78-4c83-782f4c83782f",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value"
  }
}
```





