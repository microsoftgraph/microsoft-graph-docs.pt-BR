---
title: Atualizar windowsUniversalAppX
description: Atualiza as propriedades de um objeto windowsUniversalAppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 095e06dc55f8528bb677051a0831ef91b82a4336
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754018"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="b41d5-103">Atualizar windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="b41d5-103">Update windowsUniversalAppX</span></span>

<span data-ttu-id="b41d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b41d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b41d5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b41d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b41d5-106">Atualiza as propriedades de um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="b41d5-106">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b41d5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b41d5-107">Prerequisites</span></span>
<span data-ttu-id="b41d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b41d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b41d5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b41d5-110">Permission type</span></span>|<span data-ttu-id="b41d5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b41d5-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b41d5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b41d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b41d5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b41d5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b41d5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b41d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b41d5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b41d5-115">Not supported.</span></span>|
|<span data-ttu-id="b41d5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b41d5-116">Application</span></span>|<span data-ttu-id="b41d5-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b41d5-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b41d5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b41d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b41d5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b41d5-119">Request headers</span></span>
|<span data-ttu-id="b41d5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b41d5-120">Header</span></span>|<span data-ttu-id="b41d5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b41d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b41d5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b41d5-122">Authorization</span></span>|<span data-ttu-id="b41d5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b41d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b41d5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b41d5-124">Accept</span></span>|<span data-ttu-id="b41d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b41d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b41d5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b41d5-126">Request body</span></span>
<span data-ttu-id="b41d5-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="b41d5-127">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="b41d5-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="b41d5-128">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="b41d5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b41d5-129">Property</span></span>|<span data-ttu-id="b41d5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b41d5-130">Type</span></span>|<span data-ttu-id="b41d5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b41d5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b41d5-132">id</span><span class="sxs-lookup"><span data-stu-id="b41d5-132">id</span></span>|<span data-ttu-id="b41d5-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b41d5-133">String</span></span>|<span data-ttu-id="b41d5-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b41d5-134">Key of the entity.</span></span> <span data-ttu-id="b41d5-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b41d5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b41d5-136">displayName</span></span>|<span data-ttu-id="b41d5-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b41d5-137">String</span></span>|<span data-ttu-id="b41d5-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b41d5-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b41d5-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b41d5-140">descrição</span><span class="sxs-lookup"><span data-stu-id="b41d5-140">description</span></span>|<span data-ttu-id="b41d5-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b41d5-141">String</span></span>|<span data-ttu-id="b41d5-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b41d5-142">The description of the app.</span></span> <span data-ttu-id="b41d5-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b41d5-144">publicador</span><span class="sxs-lookup"><span data-stu-id="b41d5-144">publisher</span></span>|<span data-ttu-id="b41d5-145">String</span><span class="sxs-lookup"><span data-stu-id="b41d5-145">String</span></span>|<span data-ttu-id="b41d5-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b41d5-146">The publisher of the app.</span></span> <span data-ttu-id="b41d5-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b41d5-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b41d5-148">largeIcon</span></span>|[<span data-ttu-id="b41d5-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b41d5-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b41d5-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="b41d5-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b41d5-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b41d5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b41d5-152">createdDateTime</span></span>|<span data-ttu-id="b41d5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b41d5-153">DateTimeOffset</span></span>|<span data-ttu-id="b41d5-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b41d5-154">The date and time the app was created.</span></span> <span data-ttu-id="b41d5-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b41d5-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b41d5-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b41d5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b41d5-157">DateTimeOffset</span></span>|<span data-ttu-id="b41d5-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b41d5-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b41d5-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b41d5-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b41d5-160">isFeatured</span></span>|<span data-ttu-id="b41d5-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b41d5-161">Boolean</span></span>|<span data-ttu-id="b41d5-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b41d5-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b41d5-163">privacyInformationUrl</span></span>|<span data-ttu-id="b41d5-164">String</span><span class="sxs-lookup"><span data-stu-id="b41d5-164">String</span></span>|<span data-ttu-id="b41d5-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b41d5-165">The privacy statement Url.</span></span> <span data-ttu-id="b41d5-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b41d5-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b41d5-167">informationUrl</span></span>|<span data-ttu-id="b41d5-168">String</span><span class="sxs-lookup"><span data-stu-id="b41d5-168">String</span></span>|<span data-ttu-id="b41d5-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="b41d5-169">The more information Url.</span></span> <span data-ttu-id="b41d5-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b41d5-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="b41d5-171">owner</span></span>|<span data-ttu-id="b41d5-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b41d5-172">String</span></span>|<span data-ttu-id="b41d5-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b41d5-173">The owner of the app.</span></span> <span data-ttu-id="b41d5-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b41d5-175">developer</span><span class="sxs-lookup"><span data-stu-id="b41d5-175">developer</span></span>|<span data-ttu-id="b41d5-176">String</span><span class="sxs-lookup"><span data-stu-id="b41d5-176">String</span></span>|<span data-ttu-id="b41d5-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b41d5-177">The developer of the app.</span></span> <span data-ttu-id="b41d5-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b41d5-179">notes</span><span class="sxs-lookup"><span data-stu-id="b41d5-179">notes</span></span>|<span data-ttu-id="b41d5-180">String</span><span class="sxs-lookup"><span data-stu-id="b41d5-180">String</span></span>|<span data-ttu-id="b41d5-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b41d5-181">Notes for the app.</span></span> <span data-ttu-id="b41d5-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b41d5-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="b41d5-183">publishingState</span></span>|[<span data-ttu-id="b41d5-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b41d5-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b41d5-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b41d5-185">The publishing state for the app.</span></span> <span data-ttu-id="b41d5-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="b41d5-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b41d5-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b41d5-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b41d5-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b41d5-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b41d5-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b41d5-189">committedContentVersion</span></span>|<span data-ttu-id="b41d5-190">String</span><span class="sxs-lookup"><span data-stu-id="b41d5-190">String</span></span>|<span data-ttu-id="b41d5-191">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="b41d5-191">The internal committed content version.</span></span> <span data-ttu-id="b41d5-192">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b41d5-193">fileName</span><span class="sxs-lookup"><span data-stu-id="b41d5-193">fileName</span></span>|<span data-ttu-id="b41d5-194">String</span><span class="sxs-lookup"><span data-stu-id="b41d5-194">String</span></span>|<span data-ttu-id="b41d5-195">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="b41d5-195">The name of the main Lob application file.</span></span> <span data-ttu-id="b41d5-196">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b41d5-197">size</span><span class="sxs-lookup"><span data-stu-id="b41d5-197">size</span></span>|<span data-ttu-id="b41d5-198">Int64</span><span class="sxs-lookup"><span data-stu-id="b41d5-198">Int64</span></span>|<span data-ttu-id="b41d5-199">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="b41d5-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="b41d5-200">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b41d5-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b41d5-201">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="b41d5-201">applicableArchitectures</span></span>|[<span data-ttu-id="b41d5-202">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b41d5-202">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b41d5-203">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="b41d5-203">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="b41d5-204">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="b41d5-204">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="b41d5-205">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="b41d5-205">applicableDeviceTypes</span></span>|[<span data-ttu-id="b41d5-206">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="b41d5-206">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="b41d5-207">Os tipos de dispositivos Windows nos quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="b41d5-207">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="b41d5-208">Os valores possíveis são: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="b41d5-208">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="b41d5-209">identityName</span><span class="sxs-lookup"><span data-stu-id="b41d5-209">identityName</span></span>|<span data-ttu-id="b41d5-210">String</span><span class="sxs-lookup"><span data-stu-id="b41d5-210">String</span></span>|<span data-ttu-id="b41d5-211">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="b41d5-211">The Identity Name.</span></span>|
|<span data-ttu-id="b41d5-212">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="b41d5-212">identityPublisherHash</span></span>|<span data-ttu-id="b41d5-213">String</span><span class="sxs-lookup"><span data-stu-id="b41d5-213">String</span></span>|<span data-ttu-id="b41d5-214">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="b41d5-214">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="b41d5-215">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b41d5-215">identityResourceIdentifier</span></span>|<span data-ttu-id="b41d5-216">String</span><span class="sxs-lookup"><span data-stu-id="b41d5-216">String</span></span>|<span data-ttu-id="b41d5-217">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="b41d5-217">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="b41d5-218">isBundle</span><span class="sxs-lookup"><span data-stu-id="b41d5-218">isBundle</span></span>|<span data-ttu-id="b41d5-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="b41d5-219">Boolean</span></span>|<span data-ttu-id="b41d5-220">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="b41d5-220">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="b41d5-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b41d5-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b41d5-222">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b41d5-222">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="b41d5-223">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="b41d5-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="b41d5-224">identityVersion</span><span class="sxs-lookup"><span data-stu-id="b41d5-224">identityVersion</span></span>|<span data-ttu-id="b41d5-225">String</span><span class="sxs-lookup"><span data-stu-id="b41d5-225">String</span></span>|<span data-ttu-id="b41d5-226">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="b41d5-226">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="b41d5-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="b41d5-227">Response</span></span>
<span data-ttu-id="b41d5-228">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b41d5-228">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b41d5-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b41d5-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="b41d5-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b41d5-230">Request</span></span>
<span data-ttu-id="b41d5-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b41d5-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="b41d5-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="b41d5-232">Response</span></span>
<span data-ttu-id="b41d5-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b41d5-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```




