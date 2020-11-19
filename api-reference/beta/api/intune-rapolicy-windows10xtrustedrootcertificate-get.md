---
title: Obter windows10XTrustedRootCertificate
description: Leia as propriedades e as relações do objeto windows10XTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 773e2aa0417e2b1444e9d6805dcee1e1723e44ab
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241297"
---
# <a name="get-windows10xtrustedrootcertificate"></a><span data-ttu-id="2c8bf-103">Obter windows10XTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="2c8bf-103">Get windows10XTrustedRootCertificate</span></span>

<span data-ttu-id="2c8bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c8bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c8bf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2c8bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c8bf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c8bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c8bf-107">Leia as propriedades e as relações do objeto [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="2c8bf-107">Read properties and relationships of the [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c8bf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2c8bf-108">Prerequisites</span></span>
<span data-ttu-id="2c8bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c8bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c8bf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c8bf-111">Permission type</span></span>|<span data-ttu-id="2c8bf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2c8bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c8bf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c8bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2c8bf-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c8bf-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2c8bf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c8bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c8bf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c8bf-116">Not supported.</span></span>|
|<span data-ttu-id="2c8bf-117">Application</span><span class="sxs-lookup"><span data-stu-id="2c8bf-117">Application</span></span>|<span data-ttu-id="2c8bf-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c8bf-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c8bf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c8bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c8bf-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2c8bf-120">Optional query parameters</span></span>
<span data-ttu-id="2c8bf-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2c8bf-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c8bf-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c8bf-122">Request headers</span></span>
|<span data-ttu-id="2c8bf-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2c8bf-123">Header</span></span>|<span data-ttu-id="2c8bf-124">Valor</span><span class="sxs-lookup"><span data-stu-id="2c8bf-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c8bf-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c8bf-125">Authorization</span></span>|<span data-ttu-id="2c8bf-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c8bf-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c8bf-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2c8bf-127">Accept</span></span>|<span data-ttu-id="2c8bf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2c8bf-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c8bf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c8bf-129">Request body</span></span>
<span data-ttu-id="2c8bf-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2c8bf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c8bf-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c8bf-131">Response</span></span>
<span data-ttu-id="2c8bf-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c8bf-132">If successful, this method returns a `200 OK` response code and [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c8bf-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c8bf-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c8bf-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c8bf-134">Request</span></span>
<span data-ttu-id="2c8bf-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c8bf-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

### <a name="response"></a><span data-ttu-id="2c8bf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c8bf-136">Response</span></span>
<span data-ttu-id="2c8bf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c8bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 614

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
    "id": "be0bfd01-fd01-be0b-01fd-0bbe01fd0bbe",
    "version": 7,
    "displayName": "Display Name value",
    "description": "Description value",
    "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "destinationStore": "computerCertStoreIntermediate"
  }
}
```




