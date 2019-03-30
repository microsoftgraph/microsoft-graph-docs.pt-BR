---
title: Atualizar windowsPhone81AppXBundle
description: Atualiza as propriedades de um objeto windowsPhone81AppXBundle.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c5908c8fad99a93305f6f3662339e1799bdd6e11
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988179"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="98559-103">Atualizar windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="98559-103">Update windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="98559-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="98559-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98559-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="98559-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98559-106">Atualiza as propriedades de um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="98559-106">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98559-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98559-107">Prerequisites</span></span>
<span data-ttu-id="98559-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98559-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98559-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98559-110">Permission type</span></span>|<span data-ttu-id="98559-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="98559-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98559-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98559-112">Delegated (work or school account)</span></span>|<span data-ttu-id="98559-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98559-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="98559-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98559-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98559-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98559-115">Not supported.</span></span>|
|<span data-ttu-id="98559-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98559-116">Application</span></span>|<span data-ttu-id="98559-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98559-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98559-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98559-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="98559-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98559-119">Request headers</span></span>
|<span data-ttu-id="98559-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98559-120">Header</span></span>|<span data-ttu-id="98559-121">Valor</span><span class="sxs-lookup"><span data-stu-id="98559-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98559-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="98559-122">Authorization</span></span>|<span data-ttu-id="98559-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98559-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98559-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="98559-124">Accept</span></span>|<span data-ttu-id="98559-125">application/json</span><span class="sxs-lookup"><span data-stu-id="98559-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98559-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98559-126">Request body</span></span>
<span data-ttu-id="98559-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="98559-127">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="98559-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span><span class="sxs-lookup"><span data-stu-id="98559-128">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="98559-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98559-129">Property</span></span>|<span data-ttu-id="98559-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="98559-130">Type</span></span>|<span data-ttu-id="98559-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="98559-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98559-132">id</span><span class="sxs-lookup"><span data-stu-id="98559-132">id</span></span>|<span data-ttu-id="98559-133">String</span><span class="sxs-lookup"><span data-stu-id="98559-133">String</span></span>|<span data-ttu-id="98559-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="98559-134">Key of the entity.</span></span> <span data-ttu-id="98559-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-136">displayName</span><span class="sxs-lookup"><span data-stu-id="98559-136">displayName</span></span>|<span data-ttu-id="98559-137">String</span><span class="sxs-lookup"><span data-stu-id="98559-137">String</span></span>|<span data-ttu-id="98559-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="98559-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="98559-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-140">description</span><span class="sxs-lookup"><span data-stu-id="98559-140">description</span></span>|<span data-ttu-id="98559-141">String</span><span class="sxs-lookup"><span data-stu-id="98559-141">String</span></span>|<span data-ttu-id="98559-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="98559-142">The description of the app.</span></span> <span data-ttu-id="98559-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-144">publicador</span><span class="sxs-lookup"><span data-stu-id="98559-144">publisher</span></span>|<span data-ttu-id="98559-145">String</span><span class="sxs-lookup"><span data-stu-id="98559-145">String</span></span>|<span data-ttu-id="98559-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="98559-146">The publisher of the app.</span></span> <span data-ttu-id="98559-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="98559-148">largeIcon</span></span>|[<span data-ttu-id="98559-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="98559-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="98559-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="98559-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="98559-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="98559-152">createdDateTime</span></span>|<span data-ttu-id="98559-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98559-153">DateTimeOffset</span></span>|<span data-ttu-id="98559-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="98559-154">The date and time the app was created.</span></span> <span data-ttu-id="98559-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="98559-156">lastModifiedDateTime</span></span>|<span data-ttu-id="98559-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98559-157">DateTimeOffset</span></span>|<span data-ttu-id="98559-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="98559-158">The date and time the app was last modified.</span></span> <span data-ttu-id="98559-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="98559-160">isFeatured</span></span>|<span data-ttu-id="98559-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="98559-161">Boolean</span></span>|<span data-ttu-id="98559-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="98559-163">privacyInformationUrl</span></span>|<span data-ttu-id="98559-164">String</span><span class="sxs-lookup"><span data-stu-id="98559-164">String</span></span>|<span data-ttu-id="98559-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="98559-165">The privacy statement Url.</span></span> <span data-ttu-id="98559-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="98559-167">informationUrl</span></span>|<span data-ttu-id="98559-168">String</span><span class="sxs-lookup"><span data-stu-id="98559-168">String</span></span>|<span data-ttu-id="98559-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="98559-169">The more information Url.</span></span> <span data-ttu-id="98559-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-171">owner</span><span class="sxs-lookup"><span data-stu-id="98559-171">owner</span></span>|<span data-ttu-id="98559-172">String</span><span class="sxs-lookup"><span data-stu-id="98559-172">String</span></span>|<span data-ttu-id="98559-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="98559-173">The owner of the app.</span></span> <span data-ttu-id="98559-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-175">developer</span><span class="sxs-lookup"><span data-stu-id="98559-175">developer</span></span>|<span data-ttu-id="98559-176">String</span><span class="sxs-lookup"><span data-stu-id="98559-176">String</span></span>|<span data-ttu-id="98559-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="98559-177">The developer of the app.</span></span> <span data-ttu-id="98559-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-179">notes</span><span class="sxs-lookup"><span data-stu-id="98559-179">notes</span></span>|<span data-ttu-id="98559-180">String</span><span class="sxs-lookup"><span data-stu-id="98559-180">String</span></span>|<span data-ttu-id="98559-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="98559-181">Notes for the app.</span></span> <span data-ttu-id="98559-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="98559-183">uploadState</span></span>|<span data-ttu-id="98559-184">Int32</span><span class="sxs-lookup"><span data-stu-id="98559-184">Int32</span></span>|<span data-ttu-id="98559-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="98559-185">The upload state.</span></span> <span data-ttu-id="98559-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="98559-187">publishingState</span></span>|[<span data-ttu-id="98559-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="98559-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="98559-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="98559-189">The publishing state for the app.</span></span> <span data-ttu-id="98559-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="98559-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="98559-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="98559-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="98559-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="98559-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="98559-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="98559-193">isAssigned</span></span>|<span data-ttu-id="98559-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="98559-194">Boolean</span></span>|<span data-ttu-id="98559-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="98559-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="98559-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="98559-197">roleScopeTagIds</span></span>|<span data-ttu-id="98559-198">Coleção String</span><span class="sxs-lookup"><span data-stu-id="98559-198">String collection</span></span>|<span data-ttu-id="98559-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="98559-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="98559-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98559-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="98559-201">committedContentVersion</span></span>|<span data-ttu-id="98559-202">String</span><span class="sxs-lookup"><span data-stu-id="98559-202">String</span></span>|<span data-ttu-id="98559-203">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="98559-203">The internal committed content version.</span></span> <span data-ttu-id="98559-204">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="98559-205">fileName</span><span class="sxs-lookup"><span data-stu-id="98559-205">fileName</span></span>|<span data-ttu-id="98559-206">String</span><span class="sxs-lookup"><span data-stu-id="98559-206">String</span></span>|<span data-ttu-id="98559-207">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="98559-207">The name of the main Lob application file.</span></span> <span data-ttu-id="98559-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="98559-209">size</span><span class="sxs-lookup"><span data-stu-id="98559-209">size</span></span>|<span data-ttu-id="98559-210">Int64</span><span class="sxs-lookup"><span data-stu-id="98559-210">Int64</span></span>|<span data-ttu-id="98559-211">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="98559-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="98559-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="98559-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="98559-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="98559-213">applicableArchitectures</span></span>|[<span data-ttu-id="98559-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="98559-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="98559-215">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="98559-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="98559-216">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="98559-216">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="98559-217">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="98559-217">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="98559-218">identityName</span><span class="sxs-lookup"><span data-stu-id="98559-218">identityName</span></span>|<span data-ttu-id="98559-219">String</span><span class="sxs-lookup"><span data-stu-id="98559-219">String</span></span>|<span data-ttu-id="98559-220">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="98559-220">The Identity Name.</span></span> <span data-ttu-id="98559-221">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="98559-221">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="98559-222">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="98559-222">identityPublisherHash</span></span>|<span data-ttu-id="98559-223">String</span><span class="sxs-lookup"><span data-stu-id="98559-223">String</span></span>|<span data-ttu-id="98559-224">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="98559-224">The Identity Publisher Hash.</span></span> <span data-ttu-id="98559-225">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="98559-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="98559-226">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="98559-226">identityResourceIdentifier</span></span>|<span data-ttu-id="98559-227">String</span><span class="sxs-lookup"><span data-stu-id="98559-227">String</span></span>|<span data-ttu-id="98559-228">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="98559-228">The Identity Resource Identifier.</span></span> <span data-ttu-id="98559-229">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="98559-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="98559-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="98559-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="98559-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="98559-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="98559-232">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="98559-232">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="98559-233">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="98559-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="98559-234">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="98559-234">phoneProductIdentifier</span></span>|<span data-ttu-id="98559-235">String</span><span class="sxs-lookup"><span data-stu-id="98559-235">String</span></span>|<span data-ttu-id="98559-236">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="98559-236">The Phone Product Identifier.</span></span> <span data-ttu-id="98559-237">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="98559-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="98559-238">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="98559-238">phonePublisherId</span></span>|<span data-ttu-id="98559-239">String</span><span class="sxs-lookup"><span data-stu-id="98559-239">String</span></span>|<span data-ttu-id="98559-240">A ID do editor do telefone. herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="98559-240">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="98559-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="98559-241">identityVersion</span></span>|<span data-ttu-id="98559-242">String</span><span class="sxs-lookup"><span data-stu-id="98559-242">String</span></span>|<span data-ttu-id="98559-243">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="98559-243">The identity version.</span></span> <span data-ttu-id="98559-244">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="98559-244">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="98559-245">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="98559-245">appXPackageInformationList</span></span>|<span data-ttu-id="98559-246">coleção [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="98559-246">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="98559-247">A lista de informações do pacote AppX.</span><span class="sxs-lookup"><span data-stu-id="98559-247">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="98559-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="98559-248">Response</span></span>
<span data-ttu-id="98559-249">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98559-249">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98559-250">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98559-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="98559-251">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98559-251">Request</span></span>
<span data-ttu-id="98559-252">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98559-252">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2184

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="98559-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="98559-253">Response</span></span>
<span data-ttu-id="98559-p128">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98559-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2356

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```




