---
title: Obter groupPolicyObjectFile
description: Leia propriedades e relações do objeto groupPolicyObjectFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d39a028fe46bd10c31e99da4ef407dfcb53db0a4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158966"
---
# <a name="get-grouppolicyobjectfile"></a><span data-ttu-id="47c35-103">Obter groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="47c35-103">Get groupPolicyObjectFile</span></span>

<span data-ttu-id="47c35-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47c35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47c35-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="47c35-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47c35-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47c35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47c35-107">Leia propriedades e relações do [objeto groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)</span><span class="sxs-lookup"><span data-stu-id="47c35-107">Read properties and relationships of the [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47c35-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47c35-108">Prerequisites</span></span>
<span data-ttu-id="47c35-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47c35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47c35-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47c35-111">Permission type</span></span>|<span data-ttu-id="47c35-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47c35-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47c35-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47c35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47c35-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47c35-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47c35-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47c35-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47c35-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47c35-116">Not supported.</span></span>|
|<span data-ttu-id="47c35-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47c35-117">Application</span></span>|<span data-ttu-id="47c35-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47c35-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47c35-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47c35-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyObjectFiles/{groupPolicyObjectFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47c35-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="47c35-120">Optional query parameters</span></span>
<span data-ttu-id="47c35-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="47c35-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47c35-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47c35-122">Request headers</span></span>
|<span data-ttu-id="47c35-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47c35-123">Header</span></span>|<span data-ttu-id="47c35-124">Valor</span><span class="sxs-lookup"><span data-stu-id="47c35-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47c35-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="47c35-125">Authorization</span></span>|<span data-ttu-id="47c35-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47c35-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47c35-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47c35-127">Accept</span></span>|<span data-ttu-id="47c35-128">application/json</span><span class="sxs-lookup"><span data-stu-id="47c35-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47c35-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47c35-129">Request body</span></span>
<span data-ttu-id="47c35-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47c35-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47c35-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="47c35-131">Response</span></span>
<span data-ttu-id="47c35-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47c35-132">If successful, this method returns a `200 OK` response code and [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47c35-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47c35-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="47c35-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47c35-134">Request</span></span>
<span data-ttu-id="47c35-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47c35-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyObjectFiles/{groupPolicyObjectFileId}
```

### <a name="response"></a><span data-ttu-id="47c35-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="47c35-136">Response</span></span>
<span data-ttu-id="47c35-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47c35-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
    "id": "65c0499d-499d-65c0-9d49-c0659d49c065",
    "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
    "ouDistinguishedName": "Ou Distinguished Name value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "content": "Content value"
  }
}
```




