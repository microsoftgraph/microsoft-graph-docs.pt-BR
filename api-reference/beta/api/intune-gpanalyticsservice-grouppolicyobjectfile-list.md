---
title: Listar groupPolicyObjectFiles
description: Listar propriedades e relações dos objetos groupPolicyObjectFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d5431060778506f141efcedcc40bfcf4c35781d4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158952"
---
# <a name="list-grouppolicyobjectfiles"></a><span data-ttu-id="33a4e-103">Listar groupPolicyObjectFiles</span><span class="sxs-lookup"><span data-stu-id="33a4e-103">List groupPolicyObjectFiles</span></span>

<span data-ttu-id="33a4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33a4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33a4e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="33a4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33a4e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="33a4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33a4e-107">Listar propriedades e relações dos [objetos groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)</span><span class="sxs-lookup"><span data-stu-id="33a4e-107">List properties and relationships of the [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33a4e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33a4e-108">Prerequisites</span></span>
<span data-ttu-id="33a4e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33a4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33a4e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33a4e-111">Permission type</span></span>|<span data-ttu-id="33a4e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33a4e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33a4e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33a4e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33a4e-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33a4e-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33a4e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33a4e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33a4e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33a4e-116">Not supported.</span></span>|
|<span data-ttu-id="33a4e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33a4e-117">Application</span></span>|<span data-ttu-id="33a4e-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33a4e-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33a4e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33a4e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyObjectFiles
```

## <a name="request-headers"></a><span data-ttu-id="33a4e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33a4e-120">Request headers</span></span>
|<span data-ttu-id="33a4e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33a4e-121">Header</span></span>|<span data-ttu-id="33a4e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="33a4e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33a4e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="33a4e-123">Authorization</span></span>|<span data-ttu-id="33a4e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33a4e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33a4e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="33a4e-125">Accept</span></span>|<span data-ttu-id="33a4e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33a4e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33a4e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33a4e-127">Request body</span></span>
<span data-ttu-id="33a4e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="33a4e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33a4e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="33a4e-129">Response</span></span>
<span data-ttu-id="33a4e-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33a4e-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33a4e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33a4e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="33a4e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33a4e-132">Request</span></span>
<span data-ttu-id="33a4e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33a4e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyObjectFiles
```

### <a name="response"></a><span data-ttu-id="33a4e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="33a4e-134">Response</span></span>
<span data-ttu-id="33a4e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33a4e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
      "id": "65c0499d-499d-65c0-9d49-c0659d49c065",
      "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
      "ouDistinguishedName": "Ou Distinguished Name value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "content": "Content value"
    }
  ]
}
```




