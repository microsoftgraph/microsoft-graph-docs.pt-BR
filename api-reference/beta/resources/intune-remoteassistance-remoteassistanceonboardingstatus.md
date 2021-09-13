---
title: Tipo de número remoteAssistanceOnboardingStatus
description: O status atual do conector teamViewer
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ea059025920da62824d816062fe60c03d6b5938d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039480"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>Tipo de número remoteAssistanceOnboardingStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O status atual do conector teamViewer

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notOnboarded|0|O status relatado quando não há um conector TeamViewer ativo configurado ou ativo|
|integração|1|O status relatado quando o sistema iniciou uma conexão TeamViewer, mas o serviço ainda não concluiu a confirmação de um conector|
|onboarded|2|O status relatado quando o sistema troca com êxito informações de conta com o TeamViewer e agora pode iniciar sessões de assistência remota com clientes|



