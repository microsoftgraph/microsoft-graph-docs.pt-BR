---
title: Atualizar Propriedadesdeviceconfigurationconflictsummary
description: Atualiza as propriedades de um objeto Propriedadesdeviceconfigurationconflictsummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b09b9e3ab563b0d00fed9a8dfca2eec6118641b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927402"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="886b6-103">Atualizar Propriedadesdeviceconfigurationconflictsummary</span><span class="sxs-lookup"><span data-stu-id="886b6-103">Update deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="886b6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="886b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="886b6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="886b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="886b6-106">Atualiza as propriedades de um objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="886b6-106">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="886b6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="886b6-107">Prerequisites</span></span>
<span data-ttu-id="886b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="886b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="886b6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="886b6-110">Permission type</span></span>|<span data-ttu-id="886b6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="886b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="886b6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="886b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="886b6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="886b6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="886b6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="886b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="886b6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="886b6-115">Not supported.</span></span>|
|<span data-ttu-id="886b6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="886b6-116">Application</span></span>|<span data-ttu-id="886b6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="886b6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="886b6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="886b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="886b6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="886b6-119">Request headers</span></span>
|<span data-ttu-id="886b6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="886b6-120">Header</span></span>|<span data-ttu-id="886b6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="886b6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="886b6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="886b6-122">Authorization</span></span>|<span data-ttu-id="886b6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="886b6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="886b6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="886b6-124">Accept</span></span>|<span data-ttu-id="886b6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="886b6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="886b6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="886b6-126">Request body</span></span>
<span data-ttu-id="886b6-127">No corpo da solicitação, forneça uma representação JSON do objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="886b6-127">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="886b6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="886b6-128">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="886b6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="886b6-129">Property</span></span>|<span data-ttu-id="886b6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="886b6-130">Type</span></span>|<span data-ttu-id="886b6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="886b6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="886b6-132">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="886b6-132">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="886b6-133">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="886b6-133">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="886b6-134">O conjunto de políticas em conflito com a configuração determinada</span><span class="sxs-lookup"><span data-stu-id="886b6-134">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="886b6-135">id</span><span class="sxs-lookup"><span data-stu-id="886b6-135">id</span></span>|<span data-ttu-id="886b6-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="886b6-136">String</span></span>|<span data-ttu-id="886b6-137">A ID desse conjunto de diretivas conflitantes.</span><span class="sxs-lookup"><span data-stu-id="886b6-137">The id for this set of conflicting policies.</span></span> <span data-ttu-id="886b6-138">Esta ID é as identificações de todas as políticas no ConflictingDeviceConfigurations na ordem lexicographical separadas por sublinhados.</span><span class="sxs-lookup"><span data-stu-id="886b6-138">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="886b6-139">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="886b6-139">contributingSettings</span></span>|<span data-ttu-id="886b6-140">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="886b6-140">String collection</span></span>|<span data-ttu-id="886b6-141">O conjunto de configurações em conflito com as políticas determinadas</span><span class="sxs-lookup"><span data-stu-id="886b6-141">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="886b6-142">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="886b6-142">deviceCheckinsImpacted</span></span>|<span data-ttu-id="886b6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="886b6-143">Int32</span></span>|<span data-ttu-id="886b6-144">A contagem de check-ins impactados pelas políticas e configurações conflitantes</span><span class="sxs-lookup"><span data-stu-id="886b6-144">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="886b6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="886b6-145">Response</span></span>
<span data-ttu-id="886b6-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="886b6-146">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="886b6-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="886b6-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="886b6-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="886b6-148">Request</span></span>
<span data-ttu-id="886b6-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="886b6-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
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

### <a name="response"></a><span data-ttu-id="886b6-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="886b6-150">Response</span></span>
<span data-ttu-id="886b6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="886b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




