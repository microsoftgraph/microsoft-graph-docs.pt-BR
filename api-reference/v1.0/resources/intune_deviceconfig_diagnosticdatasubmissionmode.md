# <a name="diagnosticdatasubmissionmode-enum-type"></a>tipo enumerado diagnosticDataSubmissionMode

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Permitir que o dispositivo envie dados telemétricos de diagnóstico e uso, como o Watson.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Permitir que o usuário configure.|
|none|1|Nenhum dado telemétrico enviado a partir dos componentes OS. Observação: Esse valor só é aplicável aos dispositivos de empresa e servidor. O uso dessa configuração em outros dispositivos é equivalente a definir o valor de 1.|
|basic|2|Envia dados telemétricos básicos.|
|enhanced|3|Envia dados telemétricos avançados, incluindo dados de uso e insights.|
|full|4|Envia dados telemétricos completos incluindo dados de diagnósticos, como o estado do sistema.|








