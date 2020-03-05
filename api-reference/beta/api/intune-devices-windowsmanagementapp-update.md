---
title: Atualizar windowsManagementApp
description: Atualiza as propriedades de um objeto windowsManagementApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bb61043e5377450b78b09b3bfac2bb95b5b1ae64
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467757"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="9393f-103">Atualizar windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="9393f-103">Update windowsManagementApp</span></span>

<span data-ttu-id="9393f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9393f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9393f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9393f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9393f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9393f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9393f-107">Atualiza as propriedades de um objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9393f-107">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9393f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9393f-108">Prerequisites</span></span>
<span data-ttu-id="9393f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9393f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9393f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9393f-111">Permission type</span></span>|<span data-ttu-id="9393f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9393f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9393f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9393f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9393f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9393f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9393f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9393f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9393f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9393f-116">Not supported.</span></span>|
|<span data-ttu-id="9393f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9393f-117">Application</span></span>|<span data-ttu-id="9393f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9393f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9393f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9393f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="9393f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9393f-120">Request headers</span></span>
|<span data-ttu-id="9393f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9393f-121">Header</span></span>|<span data-ttu-id="9393f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9393f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9393f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9393f-123">Authorization</span></span>|<span data-ttu-id="9393f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9393f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9393f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9393f-125">Accept</span></span>|<span data-ttu-id="9393f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9393f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9393f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9393f-127">Request body</span></span>
<span data-ttu-id="9393f-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9393f-128">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="9393f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span><span class="sxs-lookup"><span data-stu-id="9393f-129">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="9393f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9393f-130">Property</span></span>|<span data-ttu-id="9393f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9393f-131">Type</span></span>|<span data-ttu-id="9393f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9393f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9393f-133">id</span><span class="sxs-lookup"><span data-stu-id="9393f-133">id</span></span>|<span data-ttu-id="9393f-134">String</span><span class="sxs-lookup"><span data-stu-id="9393f-134">String</span></span>|<span data-ttu-id="9393f-135">Identificador exclusivo para o aplicativo de gerenciamento do Windows</span><span class="sxs-lookup"><span data-stu-id="9393f-135">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="9393f-136">availableVersion</span><span class="sxs-lookup"><span data-stu-id="9393f-136">availableVersion</span></span>|<span data-ttu-id="9393f-137">String</span><span class="sxs-lookup"><span data-stu-id="9393f-137">String</span></span>|<span data-ttu-id="9393f-138">Versão disponível do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="9393f-138">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="9393f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9393f-139">Response</span></span>
<span data-ttu-id="9393f-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9393f-140">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9393f-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9393f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="9393f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9393f-142">Request</span></span>
<span data-ttu-id="9393f-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9393f-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 112

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="9393f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9393f-144">Response</span></span>
<span data-ttu-id="9393f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9393f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
  "availableVersion": "Available Version value"
}
```





