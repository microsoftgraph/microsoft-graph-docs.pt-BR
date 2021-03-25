---
title: Atualizar managedDevice
description: Atualizar as propriedades de um objeto managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b139a6c04c560cd255de60dbb859cd040ed29608
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152380"
---
# <a name="update-manageddevice"></a><span data-ttu-id="f9128-103">Atualizar managedDevice</span><span class="sxs-lookup"><span data-stu-id="f9128-103">Update managedDevice</span></span>

<span data-ttu-id="f9128-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9128-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9128-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9128-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9128-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9128-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9128-107">Atualizar as propriedades de um objeto [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9128-107">Update the properties of a [managedDevice](../resources/intune-shared-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9128-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9128-108">Prerequisites</span></span>
<span data-ttu-id="f9128-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9128-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9128-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9128-111">Permission type</span></span>|<span data-ttu-id="f9128-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9128-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9128-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9128-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9128-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9128-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9128-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9128-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9128-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9128-116">Not supported.</span></span>|
|<span data-ttu-id="f9128-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9128-117">Application</span></span>|<span data-ttu-id="f9128-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9128-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9128-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9128-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="f9128-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9128-120">Request headers</span></span>
|<span data-ttu-id="f9128-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9128-121">Header</span></span>|<span data-ttu-id="f9128-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f9128-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9128-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9128-123">Authorization</span></span>|<span data-ttu-id="f9128-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9128-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9128-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9128-125">Accept</span></span>|<span data-ttu-id="f9128-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9128-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9128-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9128-127">Request body</span></span>
<span data-ttu-id="f9128-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9128-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-shared-manageddevice.md) object.</span></span>

<span data-ttu-id="f9128-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="f9128-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-shared-manageddevice.md).</span></span>

|<span data-ttu-id="f9128-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9128-130">Property</span></span>|<span data-ttu-id="f9128-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9128-131">Type</span></span>|<span data-ttu-id="f9128-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9128-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9128-133">id</span><span class="sxs-lookup"><span data-stu-id="f9128-133">id</span></span>|<span data-ttu-id="f9128-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9128-134">String</span></span>|<span data-ttu-id="f9128-135">Chave da entidade de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f9128-135">Key of Managed device entity.</span></span>|



## <a name="response"></a><span data-ttu-id="f9128-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9128-136">Response</span></span>
<span data-ttu-id="f9128-137">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [managedDevice](../resources/intune-shared-manageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9128-137">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-shared-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9128-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9128-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9128-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9128-139">Request</span></span>
<span data-ttu-id="f9128-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9128-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 55

{
  "@odata.type": "#microsoft.graph.managedDevice"
}
```

### <a name="response"></a><span data-ttu-id="f9128-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9128-141">Response</span></span>
<span data-ttu-id="f9128-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9128-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 104

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70"
}
```




