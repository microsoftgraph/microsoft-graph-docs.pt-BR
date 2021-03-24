---
title: Atualizar windowsManagementApp
description: Atualize as propriedades de um objeto windowsManagementApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b6fb2eb59aed83744e158a808344b1f18cf834e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126392"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="d0abf-103">Atualizar windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="d0abf-103">Update windowsManagementApp</span></span>

<span data-ttu-id="d0abf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0abf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0abf-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d0abf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0abf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0abf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0abf-107">Atualize as propriedades de um [objeto windowsManagementApp.](../resources/intune-devices-windowsmanagementapp.md)</span><span class="sxs-lookup"><span data-stu-id="d0abf-107">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0abf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d0abf-108">Prerequisites</span></span>
<span data-ttu-id="d0abf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0abf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0abf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0abf-111">Permission type</span></span>|<span data-ttu-id="d0abf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0abf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0abf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0abf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0abf-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0abf-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d0abf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0abf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0abf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0abf-116">Not supported.</span></span>|
|<span data-ttu-id="d0abf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0abf-117">Application</span></span>|<span data-ttu-id="d0abf-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0abf-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0abf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0abf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="d0abf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0abf-120">Request headers</span></span>
|<span data-ttu-id="d0abf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0abf-121">Header</span></span>|<span data-ttu-id="d0abf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d0abf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0abf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0abf-123">Authorization</span></span>|<span data-ttu-id="d0abf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0abf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0abf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d0abf-125">Accept</span></span>|<span data-ttu-id="d0abf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0abf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0abf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0abf-127">Request body</span></span>
<span data-ttu-id="d0abf-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsManagementApp.](../resources/intune-devices-windowsmanagementapp.md)</span><span class="sxs-lookup"><span data-stu-id="d0abf-128">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="d0abf-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span><span class="sxs-lookup"><span data-stu-id="d0abf-129">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="d0abf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0abf-130">Property</span></span>|<span data-ttu-id="d0abf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0abf-131">Type</span></span>|<span data-ttu-id="d0abf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0abf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0abf-133">id</span><span class="sxs-lookup"><span data-stu-id="d0abf-133">id</span></span>|<span data-ttu-id="d0abf-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0abf-134">String</span></span>|<span data-ttu-id="d0abf-135">Identificador exclusivo do aplicativo de gerenciamento do Windows</span><span class="sxs-lookup"><span data-stu-id="d0abf-135">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="d0abf-136">availableVersion</span><span class="sxs-lookup"><span data-stu-id="d0abf-136">availableVersion</span></span>|<span data-ttu-id="d0abf-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0abf-137">String</span></span>|<span data-ttu-id="d0abf-138">Versão disponível do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="d0abf-138">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="d0abf-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0abf-139">Response</span></span>
<span data-ttu-id="d0abf-140">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0abf-140">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0abf-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0abf-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0abf-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0abf-142">Request</span></span>
<span data-ttu-id="d0abf-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0abf-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 112

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="d0abf-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0abf-144">Response</span></span>
<span data-ttu-id="d0abf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0abf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




