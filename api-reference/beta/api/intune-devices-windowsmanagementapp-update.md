---
title: Atualizar windowsManagementApp
description: Atualiza as propriedades de um objeto windowsManagementApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4eb4787113d6172ee3523c463191dff0948f75d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790190"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="f9efd-103">Atualizar windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="f9efd-103">Update windowsManagementApp</span></span>

> <span data-ttu-id="f9efd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9efd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9efd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9efd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9efd-106">Atualiza as propriedades de um objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f9efd-106">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9efd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9efd-107">Prerequisites</span></span>
<span data-ttu-id="f9efd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9efd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9efd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9efd-110">Permission type</span></span>|<span data-ttu-id="f9efd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9efd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9efd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9efd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9efd-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9efd-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f9efd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9efd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9efd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9efd-115">Not supported.</span></span>|
|<span data-ttu-id="f9efd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9efd-116">Application</span></span>|<span data-ttu-id="f9efd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9efd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9efd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9efd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="f9efd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9efd-119">Request headers</span></span>
|<span data-ttu-id="f9efd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9efd-120">Header</span></span>|<span data-ttu-id="f9efd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f9efd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9efd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9efd-122">Authorization</span></span>|<span data-ttu-id="f9efd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9efd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9efd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9efd-124">Accept</span></span>|<span data-ttu-id="f9efd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9efd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9efd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9efd-126">Request body</span></span>
<span data-ttu-id="f9efd-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f9efd-127">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="f9efd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span><span class="sxs-lookup"><span data-stu-id="f9efd-128">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="f9efd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9efd-129">Property</span></span>|<span data-ttu-id="f9efd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9efd-130">Type</span></span>|<span data-ttu-id="f9efd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9efd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9efd-132">id</span><span class="sxs-lookup"><span data-stu-id="f9efd-132">id</span></span>|<span data-ttu-id="f9efd-133">String</span><span class="sxs-lookup"><span data-stu-id="f9efd-133">String</span></span>|<span data-ttu-id="f9efd-134">Identificador exclusivo para o aplicativo de gerenciamento do Windows</span><span class="sxs-lookup"><span data-stu-id="f9efd-134">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="f9efd-135">availableVersion</span><span class="sxs-lookup"><span data-stu-id="f9efd-135">availableVersion</span></span>|<span data-ttu-id="f9efd-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9efd-136">String</span></span>|<span data-ttu-id="f9efd-137">Versão disponível do aplicativo de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="f9efd-137">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="f9efd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9efd-138">Response</span></span>
<span data-ttu-id="f9efd-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9efd-139">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9efd-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9efd-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9efd-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9efd-141">Request</span></span>
<span data-ttu-id="f9efd-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9efd-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 112

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="f9efd-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9efd-143">Response</span></span>
<span data-ttu-id="f9efd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9efd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





