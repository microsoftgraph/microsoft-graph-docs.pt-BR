---
title: Obter androidTrustedRootCertificate
description: Leia as propriedades e os relacionamentos do objeto androidTrustedRootCertificate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b84b7484bb02220e6526f59a7785f005bf64c6f4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408716"
---
# <a name="get-androidtrustedrootcertificate"></a><span data-ttu-id="666d0-103">Obter androidTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="666d0-103">Get androidTrustedRootCertificate</span></span>

> <span data-ttu-id="666d0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="666d0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="666d0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="666d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="666d0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="666d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="666d0-107">Leia as propriedades e os relacionamentos do objeto [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="666d0-107">Read properties and relationships of the [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="666d0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="666d0-108">Prerequisites</span></span>
<span data-ttu-id="666d0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="666d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="666d0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="666d0-111">Permission type</span></span>|<span data-ttu-id="666d0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="666d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="666d0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="666d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="666d0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="666d0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="666d0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="666d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="666d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="666d0-116">Not supported.</span></span>|
|<span data-ttu-id="666d0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="666d0-117">Application</span></span>|<span data-ttu-id="666d0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="666d0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="666d0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="666d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidCertificateProfileBase/rootCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="optional-query-parameters"></a><span data-ttu-id="666d0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="666d0-120">Optional query parameters</span></span>
<span data-ttu-id="666d0-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="666d0-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="666d0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="666d0-122">Request headers</span></span>
|<span data-ttu-id="666d0-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="666d0-123">Header</span></span>|<span data-ttu-id="666d0-124">Valor</span><span class="sxs-lookup"><span data-stu-id="666d0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="666d0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="666d0-125">Authorization</span></span>|<span data-ttu-id="666d0-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="666d0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="666d0-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="666d0-127">Accept</span></span>|<span data-ttu-id="666d0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="666d0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="666d0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="666d0-129">Request body</span></span>
<span data-ttu-id="666d0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="666d0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="666d0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="666d0-131">Response</span></span>
<span data-ttu-id="666d0-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="666d0-132">If successful, this method returns a `200 OK` response code and [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="666d0-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="666d0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="666d0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="666d0-134">Request</span></span>
<span data-ttu-id="666d0-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="666d0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
```

### <a name="response"></a><span data-ttu-id="666d0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="666d0-136">Response</span></span>
<span data-ttu-id="666d0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="666d0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 584

{
  "value": {
    "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
    "id": "7f8d751e-751e-7f8d-1e75-8d7f1e758d7f",
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




