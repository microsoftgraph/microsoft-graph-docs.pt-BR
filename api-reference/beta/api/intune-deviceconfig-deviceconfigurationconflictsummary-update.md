---
title: Atualizar deviceConfigurationConflictSummary
description: Atualize as propriedades de um objeto deviceConfigurationConflictSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2f9bc6beef2fac86f0be79189db3bcf91f787237
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978302"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="27e12-103">Atualizar deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="27e12-103">Update deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="27e12-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="27e12-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27e12-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="27e12-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27e12-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="27e12-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27e12-107">Atualize as propriedades de um objeto [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="27e12-107">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27e12-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27e12-108">Prerequisites</span></span>
<span data-ttu-id="27e12-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27e12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27e12-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27e12-111">Permission type</span></span>|<span data-ttu-id="27e12-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27e12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27e12-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27e12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27e12-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27e12-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27e12-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27e12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27e12-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27e12-116">Not supported.</span></span>|
|<span data-ttu-id="27e12-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27e12-117">Application</span></span>|<span data-ttu-id="27e12-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27e12-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27e12-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27e12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="27e12-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27e12-120">Request headers</span></span>
|<span data-ttu-id="27e12-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27e12-121">Header</span></span>|<span data-ttu-id="27e12-122">Valor</span><span class="sxs-lookup"><span data-stu-id="27e12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27e12-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="27e12-123">Authorization</span></span>|<span data-ttu-id="27e12-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27e12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27e12-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27e12-125">Accept</span></span>|<span data-ttu-id="27e12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27e12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27e12-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27e12-127">Request body</span></span>
<span data-ttu-id="27e12-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="27e12-128">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="27e12-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="27e12-129">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="27e12-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27e12-130">Property</span></span>|<span data-ttu-id="27e12-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="27e12-131">Type</span></span>|<span data-ttu-id="27e12-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="27e12-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27e12-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="27e12-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="27e12-134">Coleção [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="27e12-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="27e12-135">O conjunto de diretivas em conflito com a configuração de determinado</span><span class="sxs-lookup"><span data-stu-id="27e12-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="27e12-136">id</span><span class="sxs-lookup"><span data-stu-id="27e12-136">id</span></span>|<span data-ttu-id="27e12-137">String</span><span class="sxs-lookup"><span data-stu-id="27e12-137">String</span></span>|<span data-ttu-id="27e12-138">A identificação para este conjunto de diretivas conflitantes.</span><span class="sxs-lookup"><span data-stu-id="27e12-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="27e12-139">Este id é as identificações de todas as políticas do ConflictingDeviceConfigurations em ordem lexicographical separada por sublinhados.</span><span class="sxs-lookup"><span data-stu-id="27e12-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="27e12-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="27e12-140">contributingSettings</span></span>|<span data-ttu-id="27e12-141">String collection</span><span class="sxs-lookup"><span data-stu-id="27e12-141">String collection</span></span>|<span data-ttu-id="27e12-142">O conjunto de configurações em conflito com as políticas de determinado</span><span class="sxs-lookup"><span data-stu-id="27e12-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="27e12-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="27e12-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="27e12-144">Int32</span><span class="sxs-lookup"><span data-stu-id="27e12-144">Int32</span></span>|<span data-ttu-id="27e12-145">A contagem de check-ins afetados pelas configurações e diretivas conflitantes</span><span class="sxs-lookup"><span data-stu-id="27e12-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="27e12-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="27e12-146">Response</span></span>
<span data-ttu-id="27e12-147">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27e12-147">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27e12-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27e12-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="27e12-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27e12-149">Request</span></span>
<span data-ttu-id="27e12-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27e12-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
Content-type: application/json
Content-length: 288

{
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

### <a name="response"></a><span data-ttu-id="27e12-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="27e12-151">Response</span></span>
<span data-ttu-id="27e12-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27e12-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





