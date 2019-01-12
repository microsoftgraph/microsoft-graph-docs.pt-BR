---
title: Atualizar windowsPhone81AppX
description: Atualize as propriedades de um objeto windowsPhone81AppX.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 78c59cf0f2aaf76e735425aa5c553f75c1ea1eb0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939704"
---
# <a name="update-windowsphone81appx"></a><span data-ttu-id="322f0-103">Atualizar windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="322f0-103">Update windowsPhone81AppX</span></span>

> <span data-ttu-id="322f0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="322f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="322f0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="322f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="322f0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="322f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="322f0-107">Atualize as propriedades de um objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="322f0-107">Update the properties of a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="322f0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="322f0-108">Prerequisites</span></span>
<span data-ttu-id="322f0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="322f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="322f0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="322f0-111">Permission type</span></span>|<span data-ttu-id="322f0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="322f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="322f0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="322f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="322f0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="322f0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="322f0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="322f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="322f0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="322f0-116">Not supported.</span></span>|
|<span data-ttu-id="322f0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="322f0-117">Application</span></span>|<span data-ttu-id="322f0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="322f0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="322f0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="322f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="322f0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="322f0-120">Request headers</span></span>
|<span data-ttu-id="322f0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="322f0-121">Header</span></span>|<span data-ttu-id="322f0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="322f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="322f0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="322f0-123">Authorization</span></span>|<span data-ttu-id="322f0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="322f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="322f0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="322f0-125">Accept</span></span>|<span data-ttu-id="322f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="322f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="322f0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="322f0-127">Request body</span></span>
<span data-ttu-id="322f0-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="322f0-128">In the request body, supply a JSON representation for the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

<span data-ttu-id="322f0-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="322f0-129">The following table shows the properties that are required when you create the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span>

|<span data-ttu-id="322f0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="322f0-130">Property</span></span>|<span data-ttu-id="322f0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="322f0-131">Type</span></span>|<span data-ttu-id="322f0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="322f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="322f0-133">id</span><span class="sxs-lookup"><span data-stu-id="322f0-133">id</span></span>|<span data-ttu-id="322f0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-134">String</span></span>|<span data-ttu-id="322f0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="322f0-135">Key of the entity.</span></span> <span data-ttu-id="322f0-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="322f0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="322f0-137">displayName</span></span>|<span data-ttu-id="322f0-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-138">String</span></span>|<span data-ttu-id="322f0-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="322f0-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="322f0-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="322f0-141">description</span><span class="sxs-lookup"><span data-stu-id="322f0-141">description</span></span>|<span data-ttu-id="322f0-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-142">String</span></span>|<span data-ttu-id="322f0-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="322f0-143">The description of the app.</span></span> <span data-ttu-id="322f0-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="322f0-145">publisher</span><span class="sxs-lookup"><span data-stu-id="322f0-145">publisher</span></span>|<span data-ttu-id="322f0-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-146">String</span></span>|<span data-ttu-id="322f0-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="322f0-147">The publisher of the app.</span></span> <span data-ttu-id="322f0-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="322f0-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="322f0-149">largeIcon</span></span>|[<span data-ttu-id="322f0-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="322f0-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="322f0-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="322f0-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="322f0-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="322f0-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="322f0-153">createdDateTime</span></span>|<span data-ttu-id="322f0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="322f0-154">DateTimeOffset</span></span>|<span data-ttu-id="322f0-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="322f0-155">The date and time the app was created.</span></span> <span data-ttu-id="322f0-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="322f0-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="322f0-157">lastModifiedDateTime</span></span>|<span data-ttu-id="322f0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="322f0-158">DateTimeOffset</span></span>|<span data-ttu-id="322f0-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="322f0-159">The date and time the app was last modified.</span></span> <span data-ttu-id="322f0-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="322f0-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="322f0-161">isFeatured</span></span>|<span data-ttu-id="322f0-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="322f0-162">Boolean</span></span>|<span data-ttu-id="322f0-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="322f0-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="322f0-164">privacyInformationUrl</span></span>|<span data-ttu-id="322f0-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-165">String</span></span>|<span data-ttu-id="322f0-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="322f0-166">The privacy statement Url.</span></span> <span data-ttu-id="322f0-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="322f0-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="322f0-168">informationUrl</span></span>|<span data-ttu-id="322f0-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-169">String</span></span>|<span data-ttu-id="322f0-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="322f0-170">The more information Url.</span></span> <span data-ttu-id="322f0-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="322f0-172">owner</span><span class="sxs-lookup"><span data-stu-id="322f0-172">owner</span></span>|<span data-ttu-id="322f0-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-173">String</span></span>|<span data-ttu-id="322f0-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="322f0-174">The owner of the app.</span></span> <span data-ttu-id="322f0-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="322f0-176">developer</span><span class="sxs-lookup"><span data-stu-id="322f0-176">developer</span></span>|<span data-ttu-id="322f0-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-177">String</span></span>|<span data-ttu-id="322f0-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="322f0-178">The developer of the app.</span></span> <span data-ttu-id="322f0-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="322f0-180">Observações</span><span class="sxs-lookup"><span data-stu-id="322f0-180">notes</span></span>|<span data-ttu-id="322f0-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-181">String</span></span>|<span data-ttu-id="322f0-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="322f0-182">Notes for the app.</span></span> <span data-ttu-id="322f0-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="322f0-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="322f0-184">uploadState</span></span>|<span data-ttu-id="322f0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="322f0-185">Int32</span></span>|<span data-ttu-id="322f0-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="322f0-186">The upload state.</span></span> <span data-ttu-id="322f0-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="322f0-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="322f0-188">publishingState</span></span>|[<span data-ttu-id="322f0-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="322f0-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="322f0-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="322f0-190">The publishing state for the app.</span></span> <span data-ttu-id="322f0-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="322f0-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="322f0-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="322f0-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="322f0-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="322f0-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="322f0-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="322f0-194">committedContentVersion</span></span>|<span data-ttu-id="322f0-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-195">String</span></span>|<span data-ttu-id="322f0-196">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="322f0-196">The internal committed content version.</span></span> <span data-ttu-id="322f0-197">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="322f0-198">fileName</span><span class="sxs-lookup"><span data-stu-id="322f0-198">fileName</span></span>|<span data-ttu-id="322f0-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-199">String</span></span>|<span data-ttu-id="322f0-200">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="322f0-200">The name of the main Lob application file.</span></span> <span data-ttu-id="322f0-201">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="322f0-202">size</span><span class="sxs-lookup"><span data-stu-id="322f0-202">size</span></span>|<span data-ttu-id="322f0-203">Int64</span><span class="sxs-lookup"><span data-stu-id="322f0-203">Int64</span></span>|<span data-ttu-id="322f0-204">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="322f0-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="322f0-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="322f0-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="322f0-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="322f0-206">applicableArchitectures</span></span>|[<span data-ttu-id="322f0-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="322f0-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="322f0-208">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="322f0-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="322f0-209">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="322f0-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="322f0-210">identityName</span><span class="sxs-lookup"><span data-stu-id="322f0-210">identityName</span></span>|<span data-ttu-id="322f0-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-211">String</span></span>|<span data-ttu-id="322f0-212">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="322f0-212">The Identity Name.</span></span>|
|<span data-ttu-id="322f0-213">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="322f0-213">identityPublisherHash</span></span>|<span data-ttu-id="322f0-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-214">String</span></span>|<span data-ttu-id="322f0-215">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="322f0-215">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="322f0-216">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="322f0-216">identityResourceIdentifier</span></span>|<span data-ttu-id="322f0-217">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-217">String</span></span>|<span data-ttu-id="322f0-218">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="322f0-218">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="322f0-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="322f0-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="322f0-220">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="322f0-220">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="322f0-221">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="322f0-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="322f0-222">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="322f0-222">phoneProductIdentifier</span></span>|<span data-ttu-id="322f0-223">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-223">String</span></span>|<span data-ttu-id="322f0-224">O identificador de produto do telefone.</span><span class="sxs-lookup"><span data-stu-id="322f0-224">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="322f0-225">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="322f0-225">phonePublisherId</span></span>|<span data-ttu-id="322f0-226">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-226">String</span></span>|<span data-ttu-id="322f0-227">A ID do fornecedor de telefone.</span><span class="sxs-lookup"><span data-stu-id="322f0-227">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="322f0-228">identityVersion</span><span class="sxs-lookup"><span data-stu-id="322f0-228">identityVersion</span></span>|<span data-ttu-id="322f0-229">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="322f0-229">String</span></span>|<span data-ttu-id="322f0-230">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="322f0-230">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="322f0-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="322f0-231">Response</span></span>
<span data-ttu-id="322f0-232">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="322f0-232">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="322f0-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="322f0-233">Example</span></span>
### <a name="request"></a><span data-ttu-id="322f0-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="322f0-234">Request</span></span>
<span data-ttu-id="322f0-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="322f0-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1362

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="322f0-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="322f0-236">Response</span></span>
<span data-ttu-id="322f0-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="322f0-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1527

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
  "identityVersion": "Identity Version value"
}
```





