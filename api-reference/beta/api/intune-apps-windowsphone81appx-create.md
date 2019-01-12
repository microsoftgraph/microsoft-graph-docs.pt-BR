---
title: Criar windowsPhone81AppX
description: Crie um novo objeto de windowsPhone81AppX.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6975fe9e029b876c46523b3e6a46ce285a34380b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974046"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="1f52e-103">Criar windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="1f52e-103">Create windowsPhone81AppX</span></span>

> <span data-ttu-id="1f52e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1f52e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f52e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1f52e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f52e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1f52e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f52e-107">Crie um novo objeto de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="1f52e-107">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1f52e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1f52e-108">Prerequisites</span></span>
<span data-ttu-id="1f52e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f52e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f52e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f52e-111">Permission type</span></span>|<span data-ttu-id="1f52e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1f52e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f52e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f52e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f52e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f52e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1f52e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f52e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f52e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f52e-116">Not supported.</span></span>|
|<span data-ttu-id="1f52e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f52e-117">Application</span></span>|<span data-ttu-id="1f52e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f52e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f52e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f52e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1f52e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f52e-120">Request headers</span></span>
|<span data-ttu-id="1f52e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f52e-121">Header</span></span>|<span data-ttu-id="1f52e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1f52e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f52e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f52e-123">Authorization</span></span>|<span data-ttu-id="1f52e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f52e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f52e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1f52e-125">Accept</span></span>|<span data-ttu-id="1f52e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f52e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f52e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f52e-127">Request body</span></span>
<span data-ttu-id="1f52e-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="1f52e-128">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="1f52e-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="1f52e-129">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="1f52e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f52e-130">Property</span></span>|<span data-ttu-id="1f52e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f52e-131">Type</span></span>|<span data-ttu-id="1f52e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f52e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f52e-133">id</span><span class="sxs-lookup"><span data-stu-id="1f52e-133">id</span></span>|<span data-ttu-id="1f52e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-134">String</span></span>|<span data-ttu-id="1f52e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1f52e-135">Key of the entity.</span></span> <span data-ttu-id="1f52e-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f52e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1f52e-137">displayName</span></span>|<span data-ttu-id="1f52e-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-138">String</span></span>|<span data-ttu-id="1f52e-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="1f52e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1f52e-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f52e-141">description</span><span class="sxs-lookup"><span data-stu-id="1f52e-141">description</span></span>|<span data-ttu-id="1f52e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-142">String</span></span>|<span data-ttu-id="1f52e-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1f52e-143">The description of the app.</span></span> <span data-ttu-id="1f52e-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f52e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="1f52e-145">publisher</span></span>|<span data-ttu-id="1f52e-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-146">String</span></span>|<span data-ttu-id="1f52e-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1f52e-147">The publisher of the app.</span></span> <span data-ttu-id="1f52e-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f52e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1f52e-149">largeIcon</span></span>|[<span data-ttu-id="1f52e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1f52e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1f52e-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="1f52e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1f52e-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f52e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f52e-153">createdDateTime</span></span>|<span data-ttu-id="1f52e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f52e-154">DateTimeOffset</span></span>|<span data-ttu-id="1f52e-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1f52e-155">The date and time the app was created.</span></span> <span data-ttu-id="1f52e-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f52e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f52e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1f52e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f52e-158">DateTimeOffset</span></span>|<span data-ttu-id="1f52e-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1f52e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1f52e-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f52e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1f52e-161">isFeatured</span></span>|<span data-ttu-id="1f52e-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="1f52e-162">Boolean</span></span>|<span data-ttu-id="1f52e-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f52e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1f52e-164">privacyInformationUrl</span></span>|<span data-ttu-id="1f52e-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-165">String</span></span>|<span data-ttu-id="1f52e-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="1f52e-166">The privacy statement Url.</span></span> <span data-ttu-id="1f52e-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f52e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1f52e-168">informationUrl</span></span>|<span data-ttu-id="1f52e-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-169">String</span></span>|<span data-ttu-id="1f52e-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="1f52e-170">The more information Url.</span></span> <span data-ttu-id="1f52e-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f52e-172">owner</span><span class="sxs-lookup"><span data-stu-id="1f52e-172">owner</span></span>|<span data-ttu-id="1f52e-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-173">String</span></span>|<span data-ttu-id="1f52e-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="1f52e-174">The owner of the app.</span></span> <span data-ttu-id="1f52e-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f52e-176">developer</span><span class="sxs-lookup"><span data-stu-id="1f52e-176">developer</span></span>|<span data-ttu-id="1f52e-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-177">String</span></span>|<span data-ttu-id="1f52e-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1f52e-178">The developer of the app.</span></span> <span data-ttu-id="1f52e-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f52e-180">Observações</span><span class="sxs-lookup"><span data-stu-id="1f52e-180">notes</span></span>|<span data-ttu-id="1f52e-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-181">String</span></span>|<span data-ttu-id="1f52e-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1f52e-182">Notes for the app.</span></span> <span data-ttu-id="1f52e-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f52e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1f52e-184">uploadState</span></span>|<span data-ttu-id="1f52e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1f52e-185">Int32</span></span>|<span data-ttu-id="1f52e-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="1f52e-186">The upload state.</span></span> <span data-ttu-id="1f52e-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f52e-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="1f52e-188">publishingState</span></span>|[<span data-ttu-id="1f52e-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1f52e-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1f52e-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1f52e-190">The publishing state for the app.</span></span> <span data-ttu-id="1f52e-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="1f52e-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1f52e-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1f52e-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1f52e-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1f52e-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1f52e-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1f52e-194">committedContentVersion</span></span>|<span data-ttu-id="1f52e-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-195">String</span></span>|<span data-ttu-id="1f52e-196">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="1f52e-196">The internal committed content version.</span></span> <span data-ttu-id="1f52e-197">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1f52e-198">fileName</span><span class="sxs-lookup"><span data-stu-id="1f52e-198">fileName</span></span>|<span data-ttu-id="1f52e-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-199">String</span></span>|<span data-ttu-id="1f52e-200">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="1f52e-200">The name of the main Lob application file.</span></span> <span data-ttu-id="1f52e-201">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1f52e-202">size</span><span class="sxs-lookup"><span data-stu-id="1f52e-202">size</span></span>|<span data-ttu-id="1f52e-203">Int64</span><span class="sxs-lookup"><span data-stu-id="1f52e-203">Int64</span></span>|<span data-ttu-id="1f52e-204">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="1f52e-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="1f52e-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f52e-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1f52e-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="1f52e-206">applicableArchitectures</span></span>|[<span data-ttu-id="1f52e-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="1f52e-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="1f52e-208">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="1f52e-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="1f52e-209">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="1f52e-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="1f52e-210">identityName</span><span class="sxs-lookup"><span data-stu-id="1f52e-210">identityName</span></span>|<span data-ttu-id="1f52e-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-211">String</span></span>|<span data-ttu-id="1f52e-212">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1f52e-212">The Identity Name.</span></span>|
|<span data-ttu-id="1f52e-213">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="1f52e-213">identityPublisherHash</span></span>|<span data-ttu-id="1f52e-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-214">String</span></span>|<span data-ttu-id="1f52e-215">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="1f52e-215">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="1f52e-216">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="1f52e-216">identityResourceIdentifier</span></span>|<span data-ttu-id="1f52e-217">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-217">String</span></span>|<span data-ttu-id="1f52e-218">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1f52e-218">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="1f52e-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1f52e-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1f52e-220">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1f52e-220">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="1f52e-221">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="1f52e-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="1f52e-222">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="1f52e-222">phoneProductIdentifier</span></span>|<span data-ttu-id="1f52e-223">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-223">String</span></span>|<span data-ttu-id="1f52e-224">O identificador de produto do telefone.</span><span class="sxs-lookup"><span data-stu-id="1f52e-224">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="1f52e-225">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="1f52e-225">phonePublisherId</span></span>|<span data-ttu-id="1f52e-226">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-226">String</span></span>|<span data-ttu-id="1f52e-227">A ID do fornecedor de telefone.</span><span class="sxs-lookup"><span data-stu-id="1f52e-227">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="1f52e-228">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1f52e-228">identityVersion</span></span>|<span data-ttu-id="1f52e-229">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f52e-229">String</span></span>|<span data-ttu-id="1f52e-230">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="1f52e-230">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="1f52e-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f52e-231">Response</span></span>
<span data-ttu-id="1f52e-232">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f52e-232">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f52e-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f52e-233">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f52e-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f52e-234">Request</span></span>
<span data-ttu-id="1f52e-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f52e-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1419

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
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

### <a name="response"></a><span data-ttu-id="1f52e-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f52e-236">Response</span></span>
<span data-ttu-id="1f52e-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f52e-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





