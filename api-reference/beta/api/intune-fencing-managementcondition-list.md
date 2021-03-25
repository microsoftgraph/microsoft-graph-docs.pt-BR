---
title: Gerenciamento de listasConditions
description: Listar propriedades e relações dos objetos managementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc92286ba3dd3713be50aa014b35e7b874a19124
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153717"
---
# <a name="list-managementconditions"></a><span data-ttu-id="2caaf-103">Gerenciamento de listasConditions</span><span class="sxs-lookup"><span data-stu-id="2caaf-103">List managementConditions</span></span>

<span data-ttu-id="2caaf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2caaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2caaf-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2caaf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2caaf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2caaf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2caaf-107">Listar propriedades e relações dos objetos [managementCondition.](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2caaf-107">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2caaf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2caaf-108">Prerequisites</span></span>
<span data-ttu-id="2caaf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2caaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2caaf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2caaf-111">Permission type</span></span>|<span data-ttu-id="2caaf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2caaf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2caaf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2caaf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2caaf-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2caaf-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2caaf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2caaf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2caaf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2caaf-116">Not supported.</span></span>|
|<span data-ttu-id="2caaf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2caaf-117">Application</span></span>|<span data-ttu-id="2caaf-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2caaf-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2caaf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2caaf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="2caaf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2caaf-120">Request headers</span></span>
|<span data-ttu-id="2caaf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2caaf-121">Header</span></span>|<span data-ttu-id="2caaf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2caaf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2caaf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2caaf-123">Authorization</span></span>|<span data-ttu-id="2caaf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2caaf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2caaf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2caaf-125">Accept</span></span>|<span data-ttu-id="2caaf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2caaf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2caaf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2caaf-127">Request body</span></span>
<span data-ttu-id="2caaf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2caaf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2caaf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2caaf-129">Response</span></span>
<span data-ttu-id="2caaf-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos managementCondition](../resources/intune-fencing-managementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2caaf-130">If successful, this method returns a `200 OK` response code and a collection of [managementCondition](../resources/intune-fencing-managementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2caaf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2caaf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2caaf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2caaf-132">Request</span></span>
<span data-ttu-id="2caaf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2caaf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="2caaf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2caaf-134">Response</span></span>
<span data-ttu-id="2caaf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2caaf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managementCondition",
      "id": "5cb49381-9381-5cb4-8193-b45c8193b45c",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```




