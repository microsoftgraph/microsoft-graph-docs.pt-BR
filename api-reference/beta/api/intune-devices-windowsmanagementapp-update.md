---
title: Atualizar windowsManagementApp
description: Atualize as propriedades de um objeto windowsManagementApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 15fea6f46279f96ce3d1f235b92475bdc67d0f16
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52662939"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="7dbac-103">Atualizar windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="7dbac-103">Update windowsManagementApp</span></span>

<span data-ttu-id="7dbac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dbac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7dbac-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7dbac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dbac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7dbac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dbac-107">Atualize as propriedades de um [objeto windowsManagementApp.](../resources/intune-devices-windowsmanagementapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dbac-107">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7dbac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7dbac-108">Prerequisites</span></span>
<span data-ttu-id="7dbac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dbac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dbac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7dbac-111">Permission type</span></span>|<span data-ttu-id="7dbac-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7dbac-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dbac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7dbac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7dbac-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dbac-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7dbac-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7dbac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dbac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dbac-116">Not supported.</span></span>|
|<span data-ttu-id="7dbac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7dbac-117">Application</span></span>|<span data-ttu-id="7dbac-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dbac-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dbac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dbac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="7dbac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7dbac-120">Request headers</span></span>
|<span data-ttu-id="7dbac-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7dbac-121">Header</span></span>|<span data-ttu-id="7dbac-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7dbac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dbac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7dbac-123">Authorization</span></span>|<span data-ttu-id="7dbac-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7dbac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dbac-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7dbac-125">Accept</span></span>|<span data-ttu-id="7dbac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7dbac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dbac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7dbac-127">Request body</span></span>
<span data-ttu-id="7dbac-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsManagementApp.](../resources/intune-devices-windowsmanagementapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dbac-128">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="7dbac-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dbac-129">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="7dbac-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7dbac-130">Property</span></span>|<span data-ttu-id="7dbac-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dbac-131">Type</span></span>|<span data-ttu-id="7dbac-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dbac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dbac-133">id</span><span class="sxs-lookup"><span data-stu-id="7dbac-133">id</span></span>|<span data-ttu-id="7dbac-134">String</span><span class="sxs-lookup"><span data-stu-id="7dbac-134">String</span></span>|<span data-ttu-id="7dbac-135">Identificador exclusivo do aplicativo Windows de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="7dbac-135">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="7dbac-136">availableVersion</span><span class="sxs-lookup"><span data-stu-id="7dbac-136">availableVersion</span></span>|<span data-ttu-id="7dbac-137">String</span><span class="sxs-lookup"><span data-stu-id="7dbac-137">String</span></span>|<span data-ttu-id="7dbac-138">Windows versão disponível do aplicativo de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7dbac-138">Windows management app available version.</span></span>|
|<span data-ttu-id="7dbac-139">managedInstaller</span><span class="sxs-lookup"><span data-stu-id="7dbac-139">managedInstaller</span></span>|[<span data-ttu-id="7dbac-140">managedInstallerStatus</span><span class="sxs-lookup"><span data-stu-id="7dbac-140">managedInstallerStatus</span></span>](../resources/intune-devices-managedinstallerstatus.md)|<span data-ttu-id="7dbac-141">Status do Instalador Gerenciado.</span><span class="sxs-lookup"><span data-stu-id="7dbac-141">Managed Installer Status.</span></span> <span data-ttu-id="7dbac-142">Os valores possíveis são: `disabled` e `enabled`.</span><span class="sxs-lookup"><span data-stu-id="7dbac-142">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="7dbac-143">managedInstallerConfiguredDateTime</span><span class="sxs-lookup"><span data-stu-id="7dbac-143">managedInstallerConfiguredDateTime</span></span>|<span data-ttu-id="7dbac-144">String</span><span class="sxs-lookup"><span data-stu-id="7dbac-144">String</span></span>|<span data-ttu-id="7dbac-145">Data configurada do Instalador Gerenciado</span><span class="sxs-lookup"><span data-stu-id="7dbac-145">Managed Installer Configured Date Time</span></span>|



## <a name="response"></a><span data-ttu-id="7dbac-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dbac-146">Response</span></span>
<span data-ttu-id="7dbac-147">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dbac-147">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dbac-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7dbac-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="7dbac-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7dbac-149">Request</span></span>
<span data-ttu-id="7dbac-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7dbac-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value",
  "managedInstaller": "enabled",
  "managedInstallerConfiguredDateTime": "Managed Installer Configured Date Time value"
}
```

### <a name="response"></a><span data-ttu-id="7dbac-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dbac-151">Response</span></span>
<span data-ttu-id="7dbac-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7dbac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
  "availableVersion": "Available Version value",
  "managedInstaller": "enabled",
  "managedInstallerConfiguredDateTime": "Managed Installer Configured Date Time value"
}
```




