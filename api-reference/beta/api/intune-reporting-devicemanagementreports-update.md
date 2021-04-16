---
title: Atualizar deviceManagementReports
description: Atualize as propriedades de um objeto deviceManagementReports.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88569f50004cbf5ec79fa6fa81457990b0356bb1
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866003"
---
# <a name="update-devicemanagementreports"></a><span data-ttu-id="31d5c-103">Atualizar deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="31d5c-103">Update deviceManagementReports</span></span>

<span data-ttu-id="31d5c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31d5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31d5c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31d5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31d5c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31d5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31d5c-107">Atualize as propriedades de [um objeto deviceManagementReports.](../resources/intune-reporting-devicemanagementreports.md)</span><span class="sxs-lookup"><span data-stu-id="31d5c-107">Update the properties of a [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31d5c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="31d5c-108">Prerequisites</span></span>
<span data-ttu-id="31d5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31d5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31d5c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31d5c-111">Permission type</span></span>|<span data-ttu-id="31d5c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31d5c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31d5c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31d5c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31d5c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31d5c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="31d5c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31d5c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31d5c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31d5c-116">Not supported.</span></span>|
|<span data-ttu-id="31d5c-117">Application</span><span class="sxs-lookup"><span data-stu-id="31d5c-117">Application</span></span>|<span data-ttu-id="31d5c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31d5c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31d5c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31d5c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports
```

## <a name="request-headers"></a><span data-ttu-id="31d5c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31d5c-120">Request headers</span></span>
|<span data-ttu-id="31d5c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31d5c-121">Header</span></span>|<span data-ttu-id="31d5c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="31d5c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31d5c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="31d5c-123">Authorization</span></span>|<span data-ttu-id="31d5c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31d5c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31d5c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="31d5c-125">Accept</span></span>|<span data-ttu-id="31d5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31d5c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31d5c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31d5c-127">Request body</span></span>
<span data-ttu-id="31d5c-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementReports.](../resources/intune-reporting-devicemanagementreports.md)</span><span class="sxs-lookup"><span data-stu-id="31d5c-128">In the request body, supply a JSON representation for the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

<span data-ttu-id="31d5c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span><span class="sxs-lookup"><span data-stu-id="31d5c-129">The following table shows the properties that are required when you create the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span></span>

|<span data-ttu-id="31d5c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31d5c-130">Property</span></span>|<span data-ttu-id="31d5c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="31d5c-131">Type</span></span>|<span data-ttu-id="31d5c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="31d5c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31d5c-133">id</span><span class="sxs-lookup"><span data-stu-id="31d5c-133">id</span></span>|<span data-ttu-id="31d5c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31d5c-134">String</span></span>|<span data-ttu-id="31d5c-135">Identificador exclusivo dessa entidade</span><span class="sxs-lookup"><span data-stu-id="31d5c-135">Unique identifier for this entity</span></span>|



## <a name="response"></a><span data-ttu-id="31d5c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="31d5c-136">Response</span></span>
<span data-ttu-id="31d5c-137">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31d5c-137">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31d5c-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31d5c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="31d5c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31d5c-139">Request</span></span>
<span data-ttu-id="31d5c-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31d5c-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```

### <a name="response"></a><span data-ttu-id="31d5c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="31d5c-141">Response</span></span>
<span data-ttu-id="31d5c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31d5c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
}
```




