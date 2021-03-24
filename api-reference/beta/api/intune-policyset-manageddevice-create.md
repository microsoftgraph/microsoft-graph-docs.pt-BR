---
title: Criar managedDevice
description: Criar um novo objeto managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5eeea35062111e7b790d767f206cfa83bab640b2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51124685"
---
# <a name="create-manageddevice"></a><span data-ttu-id="1b009-103">Criar managedDevice</span><span class="sxs-lookup"><span data-stu-id="1b009-103">Create managedDevice</span></span>

<span data-ttu-id="1b009-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b009-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b009-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1b009-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b009-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1b009-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b009-107">Criar um novo objeto [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1b009-107">Create a new [managedDevice](../resources/intune-shared-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b009-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1b009-108">Prerequisites</span></span>
<span data-ttu-id="1b009-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b009-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b009-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b009-111">Permission type</span></span>|<span data-ttu-id="1b009-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b009-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b009-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b009-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b009-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b009-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b009-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b009-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b009-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b009-116">Not supported.</span></span>|
|<span data-ttu-id="1b009-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b009-117">Application</span></span>|<span data-ttu-id="1b009-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b009-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b009-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b009-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="1b009-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b009-120">Request headers</span></span>
|<span data-ttu-id="1b009-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b009-121">Header</span></span>|<span data-ttu-id="1b009-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1b009-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b009-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b009-123">Authorization</span></span>|<span data-ttu-id="1b009-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b009-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b009-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1b009-125">Accept</span></span>|<span data-ttu-id="1b009-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b009-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b009-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b009-127">Request body</span></span>
<span data-ttu-id="1b009-128">No corpo da solicitação, forneça uma representação JSON do objeto managedDevice.</span><span class="sxs-lookup"><span data-stu-id="1b009-128">In the request body, supply a JSON representation for the managedDevice object.</span></span>

<span data-ttu-id="1b009-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDevice.</span><span class="sxs-lookup"><span data-stu-id="1b009-129">The following table shows the properties that are required when you create the managedDevice.</span></span>

|<span data-ttu-id="1b009-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b009-130">Property</span></span>|<span data-ttu-id="1b009-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b009-131">Type</span></span>|<span data-ttu-id="1b009-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b009-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b009-133">id</span><span class="sxs-lookup"><span data-stu-id="1b009-133">id</span></span>|<span data-ttu-id="1b009-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b009-134">String</span></span>|<span data-ttu-id="1b009-135">Chave da entidade de dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="1b009-135">Key of Managed device entity.</span></span>|



## <a name="response"></a><span data-ttu-id="1b009-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b009-136">Response</span></span>
<span data-ttu-id="1b009-137">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedDevice](../resources/intune-shared-manageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b009-137">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune-shared-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b009-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b009-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b009-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b009-139">Request</span></span>
<span data-ttu-id="1b009-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b009-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices
Content-type: application/json
Content-length: 55

{
  "@odata.type": "#microsoft.graph.managedDevice"
}
```

### <a name="response"></a><span data-ttu-id="1b009-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b009-141">Response</span></span>
<span data-ttu-id="1b009-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b009-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 104

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70"
}
```




