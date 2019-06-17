---
title: Criar userInstallStateSummary
description: Criar um novo objeto userInstallStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 058e5d47773172cce3f91da04f1697aa2ded3e47
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972092"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="cd7ab-103">Criar userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="cd7ab-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="cd7ab-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cd7ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd7ab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cd7ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd7ab-106">Criar um novo objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="cd7ab-106">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd7ab-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cd7ab-107">Prerequisites</span></span>
<span data-ttu-id="cd7ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd7ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd7ab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd7ab-110">Permission type</span></span>|<span data-ttu-id="cd7ab-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cd7ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd7ab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd7ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd7ab-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd7ab-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cd7ab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd7ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd7ab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd7ab-115">Not supported.</span></span>|
|<span data-ttu-id="cd7ab-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd7ab-116">Application</span></span>|<span data-ttu-id="cd7ab-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd7ab-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd7ab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd7ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="cd7ab-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd7ab-119">Request headers</span></span>
|<span data-ttu-id="cd7ab-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cd7ab-120">Header</span></span>|<span data-ttu-id="cd7ab-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cd7ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd7ab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd7ab-122">Authorization</span></span>|<span data-ttu-id="cd7ab-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd7ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd7ab-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cd7ab-124">Accept</span></span>|<span data-ttu-id="cd7ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd7ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd7ab-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd7ab-126">Request body</span></span>
<span data-ttu-id="cd7ab-127">No corpo da solicitação, forneça uma representação JSON do objeto userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="cd7ab-127">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="cd7ab-128">A tabela a seguir mostra as propriedades que são necessárias ao criar userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="cd7ab-128">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="cd7ab-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd7ab-129">Property</span></span>|<span data-ttu-id="cd7ab-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd7ab-130">Type</span></span>|<span data-ttu-id="cd7ab-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd7ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd7ab-132">id</span><span class="sxs-lookup"><span data-stu-id="cd7ab-132">id</span></span>|<span data-ttu-id="cd7ab-133">String</span><span class="sxs-lookup"><span data-stu-id="cd7ab-133">String</span></span>|<span data-ttu-id="cd7ab-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cd7ab-134">Key of the entity.</span></span>|
|<span data-ttu-id="cd7ab-135">userName</span><span class="sxs-lookup"><span data-stu-id="cd7ab-135">userName</span></span>|<span data-ttu-id="cd7ab-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd7ab-136">String</span></span>|<span data-ttu-id="cd7ab-137">Nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="cd7ab-137">User name.</span></span>|
|<span data-ttu-id="cd7ab-138">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cd7ab-138">installedDeviceCount</span></span>|<span data-ttu-id="cd7ab-139">Int32</span><span class="sxs-lookup"><span data-stu-id="cd7ab-139">Int32</span></span>|<span data-ttu-id="cd7ab-140">Contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="cd7ab-140">Installed Device Count.</span></span>|
|<span data-ttu-id="cd7ab-141">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cd7ab-141">failedDeviceCount</span></span>|<span data-ttu-id="cd7ab-142">Int32</span><span class="sxs-lookup"><span data-stu-id="cd7ab-142">Int32</span></span>|<span data-ttu-id="cd7ab-143">Falha na contagem de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="cd7ab-143">Failed Device Count.</span></span>|
|<span data-ttu-id="cd7ab-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cd7ab-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="cd7ab-145">Int32</span><span class="sxs-lookup"><span data-stu-id="cd7ab-145">Int32</span></span>|<span data-ttu-id="cd7ab-146">Sem contagem de dispositivos instalados.</span><span class="sxs-lookup"><span data-stu-id="cd7ab-146">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="cd7ab-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd7ab-147">Response</span></span>
<span data-ttu-id="cd7ab-148">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd7ab-148">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd7ab-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd7ab-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd7ab-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd7ab-150">Request</span></span>
<span data-ttu-id="cd7ab-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd7ab-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="cd7ab-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd7ab-152">Response</span></span>
<span data-ttu-id="cd7ab-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd7ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```





