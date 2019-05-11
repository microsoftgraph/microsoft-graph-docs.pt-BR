---
title: Criar Propriedadesdeviceconfigurationconflictsummary
description: Criar um novo objeto Propriedadesdeviceconfigurationconflictsummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8bcc892e895babe22da90e1e9867cce96a195c9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927360"
---
# <a name="create-deviceconfigurationconflictsummary"></a><span data-ttu-id="55977-103">Criar Propriedadesdeviceconfigurationconflictsummary</span><span class="sxs-lookup"><span data-stu-id="55977-103">Create deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="55977-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55977-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55977-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55977-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55977-106">Criar um novo objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="55977-106">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55977-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55977-107">Prerequisites</span></span>
<span data-ttu-id="55977-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55977-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55977-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55977-110">Permission type</span></span>|<span data-ttu-id="55977-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55977-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55977-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55977-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55977-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55977-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55977-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55977-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55977-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55977-115">Not supported.</span></span>|
|<span data-ttu-id="55977-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55977-116">Application</span></span>|<span data-ttu-id="55977-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55977-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55977-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55977-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="55977-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55977-119">Request headers</span></span>
|<span data-ttu-id="55977-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55977-120">Header</span></span>|<span data-ttu-id="55977-121">Valor</span><span class="sxs-lookup"><span data-stu-id="55977-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55977-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="55977-122">Authorization</span></span>|<span data-ttu-id="55977-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55977-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55977-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="55977-124">Accept</span></span>|<span data-ttu-id="55977-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55977-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55977-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55977-126">Request body</span></span>
<span data-ttu-id="55977-127">No corpo da solicitação, forneça uma representação JSON do objeto Propriedadesdeviceconfigurationconflictsummary.</span><span class="sxs-lookup"><span data-stu-id="55977-127">In the request body, supply a JSON representation for the deviceConfigurationConflictSummary object.</span></span>

<span data-ttu-id="55977-128">A tabela a seguir mostra as propriedades que são necessárias ao criar Propriedadesdeviceconfigurationconflictsummary.</span><span class="sxs-lookup"><span data-stu-id="55977-128">The following table shows the properties that are required when you create the deviceConfigurationConflictSummary.</span></span>

|<span data-ttu-id="55977-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55977-129">Property</span></span>|<span data-ttu-id="55977-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="55977-130">Type</span></span>|<span data-ttu-id="55977-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="55977-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55977-132">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="55977-132">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="55977-133">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="55977-133">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="55977-134">O conjunto de políticas em conflito com a configuração determinada</span><span class="sxs-lookup"><span data-stu-id="55977-134">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="55977-135">id</span><span class="sxs-lookup"><span data-stu-id="55977-135">id</span></span>|<span data-ttu-id="55977-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55977-136">String</span></span>|<span data-ttu-id="55977-137">A ID desse conjunto de diretivas conflitantes.</span><span class="sxs-lookup"><span data-stu-id="55977-137">The id for this set of conflicting policies.</span></span> <span data-ttu-id="55977-138">Esta ID é as identificações de todas as políticas no ConflictingDeviceConfigurations na ordem lexicographical separadas por sublinhados.</span><span class="sxs-lookup"><span data-stu-id="55977-138">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="55977-139">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="55977-139">contributingSettings</span></span>|<span data-ttu-id="55977-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="55977-140">String collection</span></span>|<span data-ttu-id="55977-141">O conjunto de configurações em conflito com as políticas determinadas</span><span class="sxs-lookup"><span data-stu-id="55977-141">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="55977-142">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="55977-142">deviceCheckinsImpacted</span></span>|<span data-ttu-id="55977-143">Int32</span><span class="sxs-lookup"><span data-stu-id="55977-143">Int32</span></span>|<span data-ttu-id="55977-144">A contagem de check-ins impactados pelas políticas e configurações conflitantes</span><span class="sxs-lookup"><span data-stu-id="55977-144">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="55977-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="55977-145">Response</span></span>
<span data-ttu-id="55977-146">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55977-146">If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55977-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55977-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="55977-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55977-148">Request</span></span>
<span data-ttu-id="55977-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55977-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```

### <a name="response"></a><span data-ttu-id="55977-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="55977-150">Response</span></span>
<span data-ttu-id="55977-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55977-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 410

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```




