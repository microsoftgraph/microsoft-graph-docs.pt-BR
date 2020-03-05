---
title: Atualizar Propriedadesdeviceconfigurationconflictsummary
description: Atualiza as propriedades de um objeto Propriedadesdeviceconfigurationconflictsummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6fa8081bd0aefd0d789f812e9d134d1865ba911e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449241"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="ef4a0-103">Atualizar Propriedadesdeviceconfigurationconflictsummary</span><span class="sxs-lookup"><span data-stu-id="ef4a0-103">Update deviceConfigurationConflictSummary</span></span>

<span data-ttu-id="ef4a0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ef4a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef4a0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ef4a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef4a0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef4a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef4a0-107">Atualiza as propriedades de um objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="ef4a0-107">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef4a0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef4a0-108">Prerequisites</span></span>
<span data-ttu-id="ef4a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef4a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef4a0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef4a0-111">Permission type</span></span>|<span data-ttu-id="ef4a0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef4a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef4a0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef4a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef4a0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef4a0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef4a0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef4a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef4a0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef4a0-116">Not supported.</span></span>|
|<span data-ttu-id="ef4a0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef4a0-117">Application</span></span>|<span data-ttu-id="ef4a0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef4a0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef4a0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef4a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="ef4a0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef4a0-120">Request headers</span></span>
|<span data-ttu-id="ef4a0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef4a0-121">Header</span></span>|<span data-ttu-id="ef4a0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ef4a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef4a0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef4a0-123">Authorization</span></span>|<span data-ttu-id="ef4a0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef4a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef4a0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ef4a0-125">Accept</span></span>|<span data-ttu-id="ef4a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef4a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef4a0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef4a0-127">Request body</span></span>
<span data-ttu-id="ef4a0-128">No corpo da solicitação, forneça uma representação JSON do objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="ef4a0-128">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="ef4a0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ef4a0-129">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="ef4a0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef4a0-130">Property</span></span>|<span data-ttu-id="ef4a0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef4a0-131">Type</span></span>|<span data-ttu-id="ef4a0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef4a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef4a0-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="ef4a0-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="ef4a0-134">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="ef4a0-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="ef4a0-135">O conjunto de políticas em conflito com a configuração determinada</span><span class="sxs-lookup"><span data-stu-id="ef4a0-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="ef4a0-136">id</span><span class="sxs-lookup"><span data-stu-id="ef4a0-136">id</span></span>|<span data-ttu-id="ef4a0-137">String</span><span class="sxs-lookup"><span data-stu-id="ef4a0-137">String</span></span>|<span data-ttu-id="ef4a0-138">A ID desse conjunto de diretivas conflitantes.</span><span class="sxs-lookup"><span data-stu-id="ef4a0-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="ef4a0-139">Esta ID é as identificações de todas as políticas no ConflictingDeviceConfigurations na ordem lexicographical separadas por sublinhados.</span><span class="sxs-lookup"><span data-stu-id="ef4a0-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="ef4a0-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="ef4a0-140">contributingSettings</span></span>|<span data-ttu-id="ef4a0-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ef4a0-141">String collection</span></span>|<span data-ttu-id="ef4a0-142">O conjunto de configurações em conflito com as políticas determinadas</span><span class="sxs-lookup"><span data-stu-id="ef4a0-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="ef4a0-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="ef4a0-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="ef4a0-144">Int32</span><span class="sxs-lookup"><span data-stu-id="ef4a0-144">Int32</span></span>|<span data-ttu-id="ef4a0-145">A contagem de check-ins impactados pelas políticas e configurações conflitantes</span><span class="sxs-lookup"><span data-stu-id="ef4a0-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="ef4a0-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef4a0-146">Response</span></span>
<span data-ttu-id="ef4a0-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef4a0-147">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef4a0-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef4a0-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef4a0-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef4a0-149">Request</span></span>
<span data-ttu-id="ef4a0-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef4a0-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ef4a0-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef4a0-151">Response</span></span>
<span data-ttu-id="ef4a0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef4a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





