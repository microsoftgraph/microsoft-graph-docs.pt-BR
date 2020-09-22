---
title: tipo de recurso macOSPrivacyAccessControlItem
description: Representa as preferências de privacidade por processo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 250d04b573097c77a63cb3f52cfed48fff64168a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084895"
---
# <a name="macosprivacyaccesscontrolitem-resource-type"></a>tipo de recurso macOSPrivacyAccessControlItem

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa as preferências de privacidade por processo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição do aplicativo, processo ou executável.|
|identificador|Cadeia de caracteres|O caminho ou a ID do pacote do aplicativo, processo ou executável.|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|Uma ID de pacote é usada para identificar um aplicativo. Um caminho é usado para identificar um processo ou executável. Os valores possíveis são: `bundleID` e `path`.|
|codeRequirement|Cadeia de caracteres|Insira o requisito de código, que pode ser obtido com o comando "codesign – display-r –" no aplicativo de terminal. Inclua tudo após "=>".|
|staticCodeValidation|Boolean|Valida estaticamente o requisito de código. Use essa configuração se o processo invalida sua assinatura de código dinâmico.|
|blockCamera|Boolean|Bloquear o acesso ao aplicativo de câmera.|
|blockMicrophone|Boolean|Bloquear o acesso ao microfone.|
|blockScreenCapture|Boolean|Bloquear o aplicativo para capturar o conteúdo da exibição do sistema. Requer o macOS 10,15 ou posterior.|
|blockListenEvent|Boolean|Bloquear o aplicativo ou processo de ouvir eventos de dispositivos de entrada, como mouse, teclado e trackpad. Requer o macOS 10,15 ou posterior.|
|speechRecognition|[habilitação](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso ao recurso de reconhecimento de fala do sistema. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|disponibilidade|[habilitação](../resources/intune-shared-enablement.md)|Permitir que o aplicativo ou processo controle o Mac por meio do subsistema de acessibilidade. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|addressBook|[habilitação](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso a informações de contato gerenciadas pelos contatos. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|calendário|[habilitação](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso a informações de evento gerenciadas pelo calendário. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|lembretes|[habilitação](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso a informações gerenciadas por lembretes. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|fotos|[habilitação](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso a imagens gerenciadas por fotos. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|mediaLibrary|[habilitação](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso a músicas e à biblioteca de mídia. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|fileProviderPresence|[habilitação](../resources/intune-shared-enablement.md)|Permitir que o aplicativo ou o processo Acesse arquivos gerenciados por uma extensão de provedor de arquivos de outro aplicativo. Requer o macOS 10,15 ou posterior. . Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyAllFiles|[habilitação](../resources/intune-shared-enablement.md)|Controlar o acesso a todos os arquivos protegidos em um dispositivo. Os arquivos podem estar em locais como emails, mensagens, aplicativos e configurações administrativas. Aplique essa configuração com cuidado. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicySystemAdminFiles|[habilitação](../resources/intune-shared-enablement.md)|Permitir que o aplicativo ou o acesse os arquivos usados na administração do sistema. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyDesktopFolder|[habilitação](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso à pasta da área de trabalho. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyDocumentsFolder|[habilitação](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso à pasta documentos. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyDownloadsFolder|[habilitação](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso à pasta downloads. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyNetworkVolumes|[habilitação](../resources/intune-shared-enablement.md)|Permitir ou bloquear o acesso a volumes de rede. Requer o macOS 10,15 ou posterior. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|systemPolicyRemovableVolumes|[habilitação](../resources/intune-shared-enablement.md)|Controlar o acesso a volumes removíveis no dispositivo, como uma unidade de disco rígido externa. Requer o macOS 10,15 ou posterior. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|CreateEvent|[habilitação](../resources/intune-shared-enablement.md)|Controlar o acesso a APIs do CoreGraphics, que são usadas para enviar CGEvents para o fluxo de eventos do sistema. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|appleEventsAllowedReceivers|coleção [macOSAppleEventReceiver](../resources/intune-deviceconfig-macosappleeventreceiver.md)|Permitir ou negar que o aplicativo ou processo envie um evento Apple restrito para outro aplicativo ou processo. Você precisará saber o identificador, o tipo de identificador e o requisito de código do aplicativo ou processo de recebimento. Esta coleção pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSPrivacyAccessControlItem",
  "displayName": "String",
  "identifier": "String",
  "identifierType": "String",
  "codeRequirement": "String",
  "staticCodeValidation": true,
  "blockCamera": true,
  "blockMicrophone": true,
  "blockScreenCapture": true,
  "blockListenEvent": true,
  "speechRecognition": "String",
  "accessibility": "String",
  "addressBook": "String",
  "calendar": "String",
  "reminders": "String",
  "photos": "String",
  "mediaLibrary": "String",
  "fileProviderPresence": "String",
  "systemPolicyAllFiles": "String",
  "systemPolicySystemAdminFiles": "String",
  "systemPolicyDesktopFolder": "String",
  "systemPolicyDocumentsFolder": "String",
  "systemPolicyDownloadsFolder": "String",
  "systemPolicyNetworkVolumes": "String",
  "systemPolicyRemovableVolumes": "String",
  "postEvent": "String",
  "appleEventsAllowedReceivers": [
    {
      "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
      "codeRequirement": "String",
      "identifier": "String",
      "identifierType": "String",
      "allowed": true
    }
  ]
}
```






